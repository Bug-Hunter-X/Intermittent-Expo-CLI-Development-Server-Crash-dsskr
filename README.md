# Expo CLI Intermittent Crash Bug

This repository demonstrates a bug encountered with the Expo CLI, where the development server would unexpectedly crash without providing any error messages in the console. The crash was random and unrelated to any specific code changes. This made debugging challenging.

## Bug Description

The Expo development server would periodically crash during development. The console would not show any error messages or warnings that could aid in identifying the cause.  Restarting the server was the only way to recover.

## Solution

The solution involved identifying and addressing potential memory leaks or resource exhaustion within the Expo application. In this case, we'll show an example by optimizing an image loading process.

## How to reproduce

1. Clone this repository.
2. Run `npm install`
3. Run `expo start`
4. Observe the server for potential crashes.

## Files

- `expoBug.js`: Demonstrates a potential inefficient image loading process, which *might* contribute to crashes in a more complex application.
- `expoBugSolution.js`:  Shows the improved image loading process that mitigates the potential resource strain.  This is a simplification and the real-world solution could require more investigation.
