# Inconsistent Styling with :has() Selector and Dynamic Content

This repository demonstrates a common issue encountered when using the CSS `:has()` selector with dynamically added or removed content.  The `:has()` selector is intended to style a parent element based on the presence of a specific child element. However, in certain situations, particularly when the child element is added or removed using JavaScript, the parent element's styling might not update reliably across different browsers.

The `bug.css` file contains the problematic CSS code.  The `solution.css` file provides a potential workaround that addresses the browser inconsistencies using JavaScript to force a style recalculation.

## How to reproduce

1. Clone this repository.
2. Open `index.html` in a web browser.
3. Observe that the parent container is not always styled consistently when adding/removing the child with class `.highlight`.

## Solution

The `solution.css` file contains a proposed workaround.