# Test Plan - Autonomous Car Lane Detection Project

## 1. Project Overview
This project implements a lane detection system using computer vision techniques with OpenCV, integrated with an Arduino-controlled vehicle. The system processes video input to detect lane lines and controls steering commands accordingly.

## 2. Test Objectives
- Verify the accuracy and robustness of lane detection under various conditions.
- Validate the correctness of steering control commands sent to Arduino.
- Ensure system stability and responsiveness during real-time processing.
- Detect and handle error scenarios gracefully (e.g., loss of lane detection).

## 3. Scope
- Functional testing of image processing pipeline (edge detection, line detection).
- Validation of control commands logic for steering.
- Integration testing between image processing and Arduino communication.
- Exclusion: Hardware testing of Arduino physical components.

## 4. Test Strategy
- Manual testing with recorded video inputs simulating various road scenarios.
- Automated unit tests for image processing functions (if applicable).
- Thread safety and concurrency tests for multi-threaded control logic.
- Boundary testing of steering command values.
- Exploratory testing to detect unexpected behaviors.

## 5. Test Environment
- Windows 10 OS with Python 3.8+
- OpenCV 4.x, NumPy, pySerial libraries installed
- Arduino Uno connected via COM port
- Test video file: "RoadCar.mp4"
- IDE: Visual Studio Code or similar

## 6. Types of Testing
- Functional Testing
- Integration Testing
- Performance Testing (real-time processing speed)
- Usability Testing (visual output correctness)
- Negative Testing (simulate missing lane lines)

## 7. Entry Criteria
- Codebase is stable and runnable without crashes.
- Video input file is available and properly configured.
- Arduino hardware connected and responsive.

## 8. Exit Criteria
- All critical test cases pass successfully.
- No unresolved critical bugs related to lane detection or control.
- Test coverage of main functional areas achieved.

## 9. Resources and Schedule
- Tester: Quynh Tran
- Testing duration: 2 weeks
- Daily testing sessions: 2 hours

## 10. Risks and Mitigation
- Risk: Hardware communication failure  
  Mitigation: Use mock serial data for initial testing.
- Risk: Varying lighting conditions affect detection  
  Mitigation: Test with diverse video inputs.

