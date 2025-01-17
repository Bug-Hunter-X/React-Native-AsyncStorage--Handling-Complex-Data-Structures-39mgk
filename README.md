# React Native AsyncStorage: Handling Complex Data Structures

This repository demonstrates a common issue in React Native when using AsyncStorage to store and retrieve complex data structures (objects and arrays).  AsyncStorage only supports storing strings, so attempting to directly store objects or arrays results in data corruption or loss.  The example shows how to properly serialize and deserialize complex data using JSON.

## Problem

Directly storing objects in AsyncStorage leads to unexpected results, often silently corrupting data.  Retrieving what appears to be the same data may result in type errors or unexpected values.

## Solution

The solution involves serializing the data to a JSON string before storage and deserializing it after retrieval.

## How to run

1. Clone the repository: `git clone ...`
2. Navigate to the directory: `cd ...`
3. Run the app using your preferred React Native method (e.g., `npx react-native run-android` or `npx react-native run-ios`).