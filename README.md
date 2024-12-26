# Unhandled Network Errors in React Native

This repository demonstrates a common issue in React Native applications: unhandled network errors.  When fetching data from an API, the application might crash or freeze if the network request fails. This example shows how to handle such errors gracefully using try...catch blocks and error states.

## The Problem

The `DataList.js` file contains a component that fetches data from a remote API.  The original implementation lacks proper error handling, resulting in an application crash if the API request fails. 

## The Solution

The `DataListSolution.js` file presents an improved version of the component.  It uses a `try...catch` block to handle potential errors during the network request. If an error occurs, it sets an error state, which is then displayed to the user. The `finally` block ensures the loading indicator is removed even if an error occurs.

## How to Run

1. Clone the repository.
2. Run `npm install` or `yarn install` to install the necessary dependencies.
3. Run `npx react-native run-android` or `npx react-native run-ios` to start the application.