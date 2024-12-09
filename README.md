# React Native TypeError: Cannot read properties of null (reading 'name')

This repository demonstrates a common React Native error: `TypeError: Cannot read properties of null (reading 'name')`.  This error arises when you attempt to access a property of an object that's currently null or undefined. This often happens when dealing with asynchronous data or improper state management.

## Bug Reproduction

The `bug.js` file contains the problematic code.  Run the app and observe the error.  It attempts to access `user.name` before the `user` object is properly populated with data.

## Solution

The `bugSolution.js` file provides a corrected version.  The key is to use optional chaining (`?.`) or nullish coalescing (`??`) to safely access the `name` property.  Additionally, error handling and state management best practices are incorporated to prevent the error in the first place.

## How to Run

1. Clone the repository.
2. Run `npm install` or `yarn install`.
3. Run the app using your preferred React Native method (e.g., `npx react-native run-android` or `npx react-native run-ios`).