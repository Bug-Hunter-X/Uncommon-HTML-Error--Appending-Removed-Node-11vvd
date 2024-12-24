# Uncommon HTML Bug: Appending Removed Node

This repository demonstrates an uncommon error that can occur in HTML when working with DOM manipulation. The bug involves attempting to append a child node to a node that has already been removed from the Document Object Model (DOM). This action will result in an error.  The solution shows how to avoid this by verifying the node's existence before attempting the append operation.

## Bug Description
The `bug.html` file contains the buggy code. The code initially displays text within a div. A button, when clicked, removes the div from the display and then attempts to re-append it. This will produce a javascript error because the re-append is done on a removed node. 

## Solution
The `bugSolution.html` file provides a corrected version of the code. The solution checks if the node is still in the DOM before attempting the append operation, preventing the error. 