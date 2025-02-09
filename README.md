# React useEffect Hook Runs on Every Render

This repository demonstrates a common React bug where the `useEffect` hook runs on every render because of a missing dependency array. This can lead to performance problems and unexpected behavior.

## Bug Description

The `useEffect` hook in the `MyComponent` component lacks a dependency array. As a result, the effect runs after every render, causing unnecessary console logs and potentially impacting performance.  This is especially problematic when dealing with expensive operations within the effect.

## Bug Solution

The solution involves adding an empty dependency array `[]` to the `useEffect` hook. This ensures the effect runs only after the initial render.