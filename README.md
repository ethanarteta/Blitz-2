# Blitz 2 Exercise Documentation

## Introduction

This documentation provides an overview of blitz-2 exercise conducted on our web server, including the observed performance metrics, the actions taken to resolve the identified issues, and the underlying purpose of the exercise.

### Purpose:
The primary purpose of blitz-2 exercise was to monitor the performance of our web server under simulated high traffic conditions and assess the impact on connectivity. By doing so, we aimed to:

1. Identify potential bottlenecks and weaknesses in our infrastructure.
2. Evaluate the need for performance optimizations.
3. Test the effectiveness of implementing a different type of instance type to improve connectivity.

## Scenario

In this exercise, we simulated a scenario in which our web server experienced a sudden surge in traffic, with 14000 concurrent user requests hitting our server simultaneously.

## Observations

### Initial Scenario :

**Connectivity:** 
- Users connected: 13,942
- Users not connected: 58

**Key Findings:**
- High CPU usage was observed under the simulated high load conditions.
  ![image](Blitz-2-images/CPU-usage.png)
- Regular Memory usage was observered under the simulared high load conditions.
  ![image](Blitz-2-images/Memory-usage.png)

