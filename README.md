# PHP Foreach Loop Modification Issue

This repository demonstrates an uncommon bug in PHP related to modifying arrays within a foreach loop using `unset()`.  The code within `bug.php` shows a function that attempts to remove all elements with the value 'a'. However, due to the way foreach handles array indices after an element is removed using `unset()`, elements might be skipped unexpectedly.

The `bugSolution.php` file provides a corrected version that demonstrates how to avoid this issue. This bug is subtle and might not be immediately obvious to PHP developers, especially when dealing with large datasets.