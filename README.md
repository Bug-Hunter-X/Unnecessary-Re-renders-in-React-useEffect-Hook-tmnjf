# Unnecessary Re-renders in React useEffect Hook

This repository demonstrates a common React bug involving the `useEffect` hook.  The provided `MyComponent` unnecessarily re-renders due to a missing dependency array in the `useEffect` hook. This leads to performance issues, especially in complex applications.

## Problem

The `useEffect` hook, without a dependency array, runs after every render. In this example, it logs the current count to the console every time the component re-renders, even though it doesn't depend on any external values.

## Solution

The solution involves adding an empty dependency array `[]` to the `useEffect` hook.  This ensures the effect runs only once after the initial render, significantly improving performance.

## How to Run

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install the necessary dependencies.
4. Run `npm start` to start the development server.