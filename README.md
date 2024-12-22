# Uncommon HTML Bug: Incorrect `document.querySelector` Usage

This repository demonstrates a subtle bug related to using `document.querySelector` in HTML to select elements by their ID. While generally robust, it can lead to unexpected behavior if the ID is not correctly formatted or contains special characters.

The bug is demonstrated in `bug.html`. The correct approach is shown in `bugSolution.html`, utilizing `document.getElementById`, which is more reliable for selecting by ID.

## How to Reproduce

1. Open `bug.html` in a web browser.
2. Observe the console output. It will show an error because the element selection failed. 
3. Open `bugSolution.html` to see the corrected version.

## Solution

The best practice is to always use `document.getElementById` when selecting elements by their ID, as it's specifically designed for this purpose and is less prone to errors caused by unusual character usage in IDs.