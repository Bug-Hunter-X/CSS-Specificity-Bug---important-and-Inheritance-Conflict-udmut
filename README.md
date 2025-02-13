# CSS Specificity Bug: !important and Inheritance Conflict

This repository demonstrates a subtle bug related to CSS specificity and the use of the `!important` flag. The bug arises from an unexpected interaction between inheritance, specificity, and `!important`.  The `bug.css` file contains the buggy code, and `bugSolution.css` shows a corrected approach.

## Bug Description

The main issue is that the `!important` declaration on the `.child` class, while seemingly overriding the style, is overridden by the more specific selector `.parent .child`. This unexpected behavior is uncommon and often leads to debugging headaches.

## Solution

The solution involves understanding CSS specificity rules and ensuring that the style with the highest specificity is applied.  In this case, we adjust the order or selector for cleaner behavior.  The `bugSolution.css` shows a possible solution by altering the selectors or removing the unnecessary `!important` declaration.