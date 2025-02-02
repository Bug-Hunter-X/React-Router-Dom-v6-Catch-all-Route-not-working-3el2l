# React Router Dom v6 Catch-all Route Issue

This repository demonstrates a problem with the catch-all route (`/*`) in React Router Dom v6.  The catch-all route is intended to handle any path that doesn't match other defined routes, but in this example, it fails to render, resulting in a blank page.

The `App.js` file contains the buggy code.  The solution is provided in `AppSolution.js`.

## Problem

When navigating to a non-existent route (e.g., `/invalid-path`), the application displays a blank page instead of rendering the `NotFound` component. 

## Solution

The solution involves ensuring the catch-all route is placed at the end of the route definitions within `Routes` in order for it to correctly catch any unmatched paths.