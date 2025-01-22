# Next.js 15 Missing Layout Bug

This repository demonstrates a common error encountered in Next.js 15 applications when using the `app` directory.  The issue arises when a page component fails to define a necessary layout.

## Problem

Next.js 15's new `app` directory introduces a stricter layout system.  If a page file doesn't provide a layout (either implicitly or explicitly), it results in runtime errors.  This example illustrates the issue with a missing layout in the `/about.js` page.

## Solution

The solution is to ensure that every page component within the `app` directory has a defined layout.  This can be done either by using a layout file (`layout.js`) in the same directory,  or by using a `layout` prop within the page component to specify a layout from a different location.