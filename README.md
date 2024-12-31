# Expo Camera in ScrollView: Rendering and Capture Issues

This repository demonstrates a common error encountered when using Expo's Camera component within a ScrollView.  The Camera component's internal mechanisms conflict with the ScrollView's rendering process, leading to issues with the camera preview and image capture.  The solution shows how to correctly integrate the Camera to avoid this problem.

## Bug

The `bug.js` file shows an implementation where the Camera is incorrectly nested inside a ScrollView.  This will result in the camera failing to render properly or function as expected.

## Solution

The `bugSolution.js` file provides a corrected implementation. Instead of nesting the Camera within the ScrollView, it's placed outside, ensuring its proper rendering and functionality. This prevents conflicts and ensures a smooth user experience.

## How to reproduce the bug
1. Clone this repository.
2. Run `npm install`.
3. Run `expo start`.
4. Observe that the camera in `bug.js` is not rendering or working correctly.
5. Navigate to `bugSolution.js` to see the corrected implementation and properly working camera.