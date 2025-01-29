# Uncommon HTML Bug: Accessing Non-Existent Property Before Parsing

This repository demonstrates an uncommon bug in HTML related to accessing non-existent properties on DOM elements before the browser has fully parsed them.  This can lead to unexpected behavior or errors, depending on the browser and context.

The `bug.html` file shows the buggy code, and `bugSolution.html` provides a corrected version.

## Bug Description
Attempting to access a property of a DOM element before the browser has finished parsing the HTML may result in unexpected results or errors. This is not always apparent and can be difficult to debug.

## Solution
The solution involves checking for the existence of the property before attempting to access it using `hasOwnProperty()`.