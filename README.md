# Next.js 15 Runtime Error: Returning Primitive Value from Page Component

This repository demonstrates a common runtime error in Next.js 15 that occurs when a page component returns a primitive value (like a string, number, or boolean) instead of a valid React element.  Next.js 15 requires that page components always return JSX.

## Steps to Reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run `npm run dev`.
4. Navigate to `/about`.

You'll observe a runtime error in the browser console.

## Solution

Ensure that all page components in your Next.js application always return a valid React element.  Wrap primitive values in a React fragment or a suitable component like `<div>` or `<p>`.

## Additional notes

This error can be particularly tricky to debug because it's a runtime error, not a compile-time error.  Make sure to thoroughly test your Next.js application and pay attention to the console logs for any such errors.