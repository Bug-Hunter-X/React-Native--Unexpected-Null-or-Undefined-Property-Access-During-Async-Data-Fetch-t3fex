# React Native: Unexpected Null or Undefined Property Access During Async Data Fetch

This repository demonstrates a common error in React Native applications: attempting to access a property of an object that is null or undefined.  This often arises when working with asynchronous data fetching where UI components render before data has fully loaded.

## Problem

The `bug.js` file showcases the problematic code. The component tries to access `data.someProperty` before the `data` state variable is populated from the API response.  This results in a runtime error.

## Solution

The `bugSolution.js` file provides a solution using optional chaining and nullish coalescing. These operators gracefully handle null or undefined values preventing the error.  The solution demonstrates best practices for handling asynchronous operations in React Native.

## How to Run

1. Clone the repository.
2. Navigate to the project directory.
3. Run `npm install` to install dependencies.
4. Run `npx react-native run-android` or `npx react-native run-ios` to run the app on an emulator or device.

This example helps illustrate how to prevent and handle null or undefined property accesses in your React Native projects, making your apps more robust and less prone to unexpected crashes.