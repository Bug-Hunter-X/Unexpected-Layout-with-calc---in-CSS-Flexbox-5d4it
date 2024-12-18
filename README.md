# Unexpected Layout with calc() in CSS Flexbox

This repository demonstrates a common issue encountered when using the `calc()` function in CSS, specifically within flexbox layouts. The problem arises from an incorrect understanding of how `calc()` interacts with the computed width of an element.

## Bug Description

The `calc()` function is used to perform calculations within CSS. However, when used improperly within flexbox, it can lead to unexpected layout behaviors.  If you attempt to calculate a width based on the parent container's width without explicitly setting the element's width to 100%, the calculation may be based on the element's default computed width, resulting in incorrect dimensions.

## Solution

The solution involves ensuring the element has its width explicitly set to 100% before using `calc()` to calculate its final width. This way, the `calc()` function operates on the intended reference width.

## How to reproduce

1. Clone the repository.
2. Open `bug.html` in your browser.
3. Observe the unexpected layout.
4. Open `bugSolution.html` in your browser and see the corrected layout.