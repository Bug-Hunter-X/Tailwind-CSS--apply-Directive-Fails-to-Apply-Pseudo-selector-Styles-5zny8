# Tailwind CSS @apply Directive Bug

This repository demonstrates a bug where Tailwind CSS's `@apply` directive doesn't correctly apply styles when using pseudo-selectors like `:hover` or `:focus` within the applied class.  The `hover` state styles are not working as expected.

## Bug Description

The `@apply` directive is a powerful feature of Tailwind CSS but it fails to apply styles for pseudo-selectors correctly leading to unexpected behavior.

## Steps to Reproduce

1. Clone the repository.
2. Open `index.html` in your browser.
3. Observe that the button doesn't change color on hover, as expected.

## Solution

The solution involves not using `@apply` and instead directly applying the classes in the HTML.

## Additional Notes

This issue highlights a limitation of the `@apply` directive when working with pseudo-selectors. As such, using it with pseudo selectors is not recommended.  You should instead apply these classes directly in your HTML or use a different approach such as JavaScript to handle those pseudo states.