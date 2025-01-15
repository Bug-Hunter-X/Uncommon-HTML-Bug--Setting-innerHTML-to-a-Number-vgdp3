# Uncommon HTML Bug: Setting innerHTML to a Number

This repository demonstrates an uncommon bug in HTML where attempting to set the `innerHTML` property of an element to a number instead of a string leads to unexpected behavior.  The bug is subtle and may not always result in an obvious error message.

## Bug Description
The issue arises when you try to directly assign a number to the `innerHTML` property of an HTML element.  Browsers expect a string, and the behavior when a number is provided may vary slightly among different browsers. This can lead to unexpected rendering or no changes at all.

## Solution
The solution involves converting the number to a string before assigning it to `innerHTML`.  This ensures that the browser receives the expected data type.

## How to Reproduce
1. Clone this repository.
2. Open `bug.html` in your web browser.
3. Observe that the text "This text will be replaced." is not replaced with the number 123 as expected.
4. Open `bugSolution.html` to see the corrected code and the expected behavior.