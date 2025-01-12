# Expo CLI Installation Error: Cannot find module 'expo-status-bar'

This repository demonstrates a common error encountered when using the Expo CLI: the inability to find the 'expo-status-bar' module.  This typically occurs due to an issue with the project setup or missing dependencies.

## Problem

The error message 'Cannot find module 'expo-status-bar'' indicates that the project cannot locate the necessary module. This often happens after a fresh install or if dependencies are corrupted.

## Solution

The solution involves verifying the project dependencies and reinstalling the missing packages.  This example uses npm; if using yarn, substitute `npm` with `yarn`.

1. **Check `package.json`**: Ensure that `expo-status-bar` is listed as a dependency in the `dependencies` section of your `package.json` file.
2. **Install dependencies**: Run `npm install` to install or reinstall all project dependencies. This will fetch `expo-status-bar` and other required packages.
3. **Clear cache (optional)**: If the issue persists, try clearing the Expo cache using `expo start --clear`. This can help resolve inconsistencies.
4. **Check Expo SDK version**:  Make sure your Expo SDK version is compatible with `expo-status-bar`.  Check the `expo-status-bar` documentation for compatibility information.
5. **Check file paths**: Double-check that your import statement correctly references the `expo-status-bar` module; typos can lead to import errors.