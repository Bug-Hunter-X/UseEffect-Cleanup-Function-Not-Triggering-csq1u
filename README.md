# React useEffect Cleanup Function Issue

This repository demonstrates a problem with the cleanup function in React's `useEffect` hook.  The expected behavior is that the console logs within the cleanup function should be displayed when the component unmounts. However, this is not happening.

## Problem Description

The `useEffect` hook is used with an empty dependency array (`[]`), indicating that it should run only once after the initial render. The cleanup function is intended to perform actions when the component unmounts, but it appears to be inactive.

## Solution

The solution involves ensuring that the component actually unmounts in a controlled test environment. This can be achieved by replacing the component with another one or by using a test environment that can effectively render and unrender the component.