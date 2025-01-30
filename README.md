# CSS `calc()` Pitfalls: Unexpected Behavior with Dynamic Percentages

This repository demonstrates a subtle but important issue related to using the CSS `calc()` function with percentages, especially when the parent element's width is dynamic or not explicitly defined.  The issue occurs because `calc()` needs to resolve the parent width before it can correctly compute the child's width. In scenarios where the parent's width is not fully determined, this calculation can produce unexpected results.

## Bug Report

The `bug.css` file contains a CSS rule demonstrating the problematic behavior.  Observe how the `.container`'s width behaves depending on the parent container's size and whether or not the parent container has explicitly defined width.  The behavior might vary across browsers and situations.

## Solution

The `bugSolution.css` file provides a possible solution. The solution might involve alternative layout techniques or approaches which can be more reliable when dealing with dynamic dimensions. 

## How to reproduce

1. Clone this repository.
2. Open `bug.html` in your browser (You may need to create a simple HTML file to test the stylesheet).
3. Observe the behavior of the `.container` element.
4. Compare this behavior to the behavior provided in `bugSolution.html`