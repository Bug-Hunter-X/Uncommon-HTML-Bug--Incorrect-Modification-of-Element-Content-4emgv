# Uncommon HTML Bug: Incorrect Modification of Element Content

This repository demonstrates an uncommon bug in HTML related to modifying the content of an element using the `textContent` property instead of `innerHTML`.

## Bug Description
The bug arises when trying to update the content of an HTML element using `textContent`. If the new content includes HTML tags, they will be treated as plain text rather than rendered as HTML elements.

## Bug Reproduction
1. Open `bug.html` in a web browser.
2. Observe the initial content of the div element.
3. The javascript code attempts to modify content of div element using `textContent`.  Note that the modified content is not rendered properly because of the use of `textContent`.
4. The second modification is done using `innerHTML` and the content is rendered properly. 

## Solution
The solution involves using the `innerHTML` property to modify the content of the HTML element which handles and renders html tags correctly. Open `bugSolution.html` to see the correct implementation. 
