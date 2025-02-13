# React Router v6 Catch-all Route Issue

This repository demonstrates a common issue in React Router v6 where a catch-all route (`/*`) interferes with other routes, causing them to become unreachable. 

The problem stems from the order of routes defined within the `Routes` component. The catch-all route should ideally be placed last to ensure other specific routes are matched first.  If placed earlier, it will capture all paths preventing the correct rendering of other components.