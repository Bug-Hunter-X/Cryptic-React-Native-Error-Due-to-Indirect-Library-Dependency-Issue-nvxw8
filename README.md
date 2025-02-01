# Cryptic React Native Error Due to Indirect Library Dependency Issue

This repository demonstrates an uncommon React Native bug where an error is caused not by the library you are directly using, but by a missing or incorrectly linked dependency of that library.  This often leads to confusing error messages that don't directly point to the root cause.

## Problem
The `indirectDependencyBug.js` file shows an example where integrating a hypothetical mapping library (`react-native-map-lib`) leads to an error because of a missing dependency within `react-native-map-lib` (e.g., a missing `react-native-geolocation-service` dependency).  The error message might be unrelated to the mapping library itself.

## Solution
The `indirectDependencySolution.js` file demonstrates the solution: ensuring that all transitive dependencies are correctly installed and linked using tools like `npm` or `yarn`.