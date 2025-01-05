# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook. The bug causes an infinite loop, leading to performance degradation and potential application crashes.

## Bug Description
The `useEffect` hook, when used improperly, can lead to an infinite loop. This occurs when the effect's dependency array is missing or incorrectly defined. In this example, the effect is unintentionally triggered after every render, causing a continuous loop.

## Bug Reproduction
1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe the console output, showing the 'Count changed' message repeatedly, indicating the infinite loop.

## Solution
The solution involves correctly specifying the dependencies within the dependency array. The effect should only run when the relevant state variable changes.

## Contributing
Contributions are welcome! Please feel free to open issues or submit pull requests.