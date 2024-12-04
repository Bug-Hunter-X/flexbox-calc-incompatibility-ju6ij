# Flexbox and `calc()` Incompatibility

This example demonstrates an unexpected behavior when using `calc()` within a flexbox container whose width isn't explicitly set.  The `calc()` function may not produce the expected result, leading to layout issues.

The `bug.css` file contains the problematic code, while `solution.css` offers a fix.

## Bug
In the `bug.css` file, the width of the inner element is calculated as `100% - 10px`. If the flex container's width is not defined, `calc()` may not compute correctly. 

## Solution
The solution (`solution.css`) addresses this by explicitly setting the width of the flex container.