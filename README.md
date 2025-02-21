# React Router v6 Catch-All Route Bug

This repository demonstrates a common issue encountered when using the catch-all route (`/*`) in React Router v6. The catch-all route, intended to handle 404 errors, is incorrectly overriding other, more specific routes.

## Issue Description

The problem lies in the order of routes defined within `Routes`. Even when a path is more specific, the catch-all route will match it first, preventing the correct component from rendering.

## Solution

The solution is to place the catch-all route last in the `Routes` component. This ensures it only matches paths that don't match any of the preceding routes.

## Setup

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install dependencies.
4. Run `npm start` to start the development server.

This will allow you to see the issue in action and the corrected version side-by-side.