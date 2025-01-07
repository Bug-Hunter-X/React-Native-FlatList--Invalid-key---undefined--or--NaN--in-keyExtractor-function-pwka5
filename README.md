# React Native FlatList KeyExtractor Error

This repository demonstrates a common error encountered when using the `FlatList` component in React Native: providing an incorrect or missing `keyExtractor` function.

The `keyExtractor` is vital for `FlatList`'s performance and accurate rendering.  If you don't provide one, or if your `keyExtractor` returns non-unique or invalid keys, you'll likely face issues such as incorrect item updates, deletions, or performance problems.

## Bug Description

The `bug.js` file illustrates the problem: a `FlatList` is rendered without a valid `keyExtractor`. This leads to the error `Invalid key: 
undefined` or `NaN` in keyExtractor function`.

## Solution

The `bugSolution.js` file presents the corrected code. The addition of a proper `keyExtractor` function that returns a unique string identifier for each item resolves the issue. This ensures that `FlatList` can efficiently manage and update the list items correctly.