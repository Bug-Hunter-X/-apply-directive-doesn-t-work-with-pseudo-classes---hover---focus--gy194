# Tailwind CSS @apply Directive Bug with Pseudo-classes

This repository demonstrates a bug where Tailwind CSS's `@apply` directive fails to correctly apply styles when combined with pseudo-classes such as `:hover` or `:focus`.  The issue is that the `@apply` directive doesn't properly handle the cascading nature of pseudo-classes and might not apply the correct style at the expected time.

## Steps to Reproduce

1. Clone this repository.
2. Open `bug.html` in your browser.
3. Observe that the button's background color does not change on hover, even though the styles are defined correctly.
4. Compare to the `solution.html` which shows correct application of the style with a more traditional approach.

## Solution

The workaround is to avoid using `@apply` with pseudo-classes and instead apply the classes directly to the element and use the appropriate class names for hover and focus states.

This bug has been reported to the Tailwind CSS team and may be addressed in future versions. Until then, consider using the approach shown in `solution.html` to work around the issue.