# CSS Specificity Bug with !important

This repository demonstrates a subtle bug related to CSS specificity and the `!important` declaration.  The bug highlights a scenario where a more specific selector is unexpectedly overridden by a less specific one due to the use of `!important`.

## Bug Description
The provided CSS code contains two selectors that target paragraph elements (`p`) within a container.  One selector is more specific (`#container p`), while the other is less specific (`p`). The less specific selector, however, includes the `!important` flag, which overrides the more specific selector.

## How to Reproduce
1. Open `bug.css`.
2. Observe the unexpected styling applied to paragraphs within the container. The less specific selector wins due to `!important`.
3. Open `bugSolution.css` to see how to fix the issue.

## Solution
The solution involves understanding and carefully managing CSS specificity and avoiding overreliance on the `!important` declaration.