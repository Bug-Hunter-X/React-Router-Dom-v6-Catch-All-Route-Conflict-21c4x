# React Router Dom v6 Catch All Route Conflict

This repository demonstrates a common issue encountered when using the catch-all route (`/*`) in React Router Dom v6.  The catch-all route, intended to handle any unmatched routes, can unexpectedly interfere with other routes if not implemented correctly.

The provided example shows how defining `/*` as the last route in the `Routes` component can resolve the conflict. In the original `App.js`, the catch-all route is placed after other more specific routes, causing them to be ignored and only the catch-all route to render, even for defined paths.  The solution in `AppSolution.js` corrects this behavior.