# React Router Dom: Handling Unmatched Routes

This repository demonstrates a common issue in React Router Dom v6 and above and provides a solution. The problem occurs when navigating to a route that doesn't have a corresponding `<Route>` component defined. Without proper handling, the app might render nothing or display an error.

## Problem

The provided `App.js` demonstrates an application that only defines routes for `/` and `/about`. Navigating to any other path (e.g., `/contact`) leads to unexpected behavior because no route handles this unmatched path.

## Solution

The `AppSolution.js` file provides a solution by adding a `Route` with a `path="*"` to catch all unmatched routes.  This ensures a graceful fallback, preventing errors or blank screens.