# React Native - Handling 'Cannot read properties of undefined' Errors

This repository demonstrates a common error in React Native: `Cannot read properties of undefined (reading 'name')` and provides a solution.

The `bug.js` file showcases the error, while `bugSolution.js` provides a robust solution using optional chaining and nullish coalescing.

## Problem

The error `Cannot read properties of undefined (reading 'name')` arises when you attempt to access a property (like `name`) of an object that's currently `undefined` or `null`. This often happens when dealing with asynchronous data fetching in React Native, where components might render before data is fully loaded.

## Solution

The best way to avoid this is to use optional chaining (`?.`) and the nullish coalescing operator (`??`). These help you gracefully handle cases where the data might not be available yet.

## How to run

1. Clone the repository
2. Navigate to the project directory
3. Run `npm install`
4. Run `npx react-native run-android` or `npx react-native run-ios`