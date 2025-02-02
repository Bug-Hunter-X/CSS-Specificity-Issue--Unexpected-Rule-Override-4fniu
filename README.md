# CSS Specificity Bug

This repository demonstrates a subtle bug related to CSS specificity.  In some browsers, the order of rules and the way specificity is calculated can lead to unexpected results where a less-specific rule overrides a more specific one.

The `bug.css` file contains the problematic code. The `bugSolution.css` file presents a possible solution.

**Problem:** The expected behavior based on CSS specificity is that the red color should be applied to the element with the ID `parent` and class `child`. However, the green color unexpectedly overrides this due to a quirk in how some browsers handle rule order and specificity calculations.

**Solution:**  The solution involves improving code structure to avoid relying on potentially inconsistent behavior.  Reordering the rules might sometimes 'fix' the issue, but it is a bad practice. A better approach would be to ensure rules are structured to minimize ambiguity and to always verify styling across various browsers during testing. 