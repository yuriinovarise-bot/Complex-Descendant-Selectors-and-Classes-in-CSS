Complex Descendant Selectors and Classes in CSS
Description

You can create more specific CSS rules by combining descendant selectors with classes. This allows you to target elements based on both their type and the classes of their parents or themselves.

Example HTML
<div class="block">
    <h2 class="header">Title h2</h2>
    <p>text</p>

    <h3 class="header">Title h3</h3>
    <p>text</p>
    <p>text</p>
</div>
<div class="block">
    <h2 class="header">Title h2</h2>
    <p>text</p>

    <h3 class="header">Title h3</h3>
    <p>text</p>
    <p>text</p>
</div>

Example CSS
.block .header {
    font-family: Arial; /* All elements with class header inside .block */
}
.block h2.header {
    font-size: 30px;
    color: red; /* h2 elements with class header inside .block */
}
.block h3.header {
    font-size: 20px;
    color: green; /* h3 elements with class header inside .block */
}


.block .header selects all elements with class header inside .block, regardless of the tag.

.block h2.header selects h2 elements with class header inside .block.

.block h3.header selects h3 elements with class header inside .block.

This approach allows you to style different types of elements differently while still being within the same parent class.

Tasks

Explain what the selector .eee .bbb selects, and write HTML code that matches it.

Explain what the selector .eee h2 selects, and write HTML code that matches it.

Explain what the selector .eee h2.bbb selects, and write HTML code that matches it.

Explain what the selector .eee h3.bbb selects, and write HTML code that matches it.

Explain what the selector .eee p.bbb selects, and write HTML code that matches it.

Explain what the selector .eee .bbb .kkk selects, and write HTML code that matches it.
