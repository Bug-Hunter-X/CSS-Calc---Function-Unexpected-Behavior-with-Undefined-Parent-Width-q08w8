# CSS Calc() Function Unexpected Behavior

This repository demonstrates an uncommon issue related to the `calc()` function in CSS. Specifically, it highlights the problem that arises when using `calc()` to determine an element's width based on its parent's width, but the parent's width is not explicitly defined.

## The Problem

When the parent element does not have a defined width, the calculation within `calc()` might not work as expected. The `100%` value in the calculation is relative to the parent's width; if the parent's width is not set, the calculation will not produce the expected result. This can result in layout problems, such as elements not being displayed correctly.

## Solution

The solution is simple: Ensure that the parent element has a defined width, either explicitly using `width` or implicitly through other CSS properties that determine its dimensions.  You may also choose a more appropriate calculation technique that does not rely on the parent's width if a defined parent width is not always guaranteed.