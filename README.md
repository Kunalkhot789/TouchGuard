
# TouchGuard 🚨
### Real-Time Hand Proximity & Danger Alert System

## Overview
TouchGuard is a real-time computer vision prototype that tracks a user's hand using a live camera feed and detects proximity to a virtual object on screen.

The system dynamically classifies interaction into SAFE, WARNING, and DANGER states and displays clear visual alerts including "DANGER DANGER" when the hand reaches the critical boundary.

## Features
- Real-time hand / fingertip tracking (CPU-only)
- No pose-detection APIs (no MediaPipe, OpenPose)
- Classical Computer Vision (contours, convex hull, distance logic)
- Virtual boundary visualization
- Distance-based interaction states
- On-screen alert overlays
- ≥8 FPS performance on CPU

## Interaction States
- **SAFE** – Hand far from virtual object
- **WARNING** – Hand approaching boundary
- **DANGER** – Hand touching / extremely close

## Technologies Used
- Python
- OpenCV
- NumPy

## How It Works
1. Camera feed captured via OpenCV
2. Hand segmented using classical CV techniques
3. Hand contour and centroid extracted
4. Distance measured to virtual boundary
5. State classified based on distance thresholds
6. Visual feedback rendered in real time
