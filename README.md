# Unexpected Double Styling with :focus and :focus-visible

This repository demonstrates an uncommon issue with the CSS `:focus-visible` pseudo-class. The problem arises when both `:focus` and `:focus-visible` are used on the same element, leading to unexpected double styling when focusing with the keyboard. The intended behavior of `:focus-visible` is to only apply styles when focus is explicitly from the keyboard, but the `:focus` styling still prevails, and both are applied together.

## Bug
The `bug.css` file contains the CSS code that exhibits the issue.  Observe the double styling effect when interacting with the element using both the mouse and keyboard. 

## Solution
The `bugSolution.css` file demonstrates a solution by correctly ordering and utilizing the `:focus-within` pseudo-class. This ensures that styles only apply when the element or a descendant receives keyboard focus.