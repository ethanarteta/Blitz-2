# Blitz 2 Exercise Documentation

## Introduction

This documentation provides an overview of blitz-2 exercise conducted on our web server, including the observed performance metrics, the actions taken to resolve the identified issues, and the underlying purpose of the exercise.

### Purpose:
The primary purpose of blitz-2 exercise was to monitor the performance of our web server under simulated high traffic conditions and assess the impact on connectivity. By doing so, we aimed to:

1. Identify potential bottlenecks and weaknesses in our infrastructure.
2. Evaluate the need for performance optimizations.
3. Test the effectiveness of implementing a different type of instance type to improve connectivity and prevent any requests to time out or fail to be processed all together.

## Scenario

In this exercise, we simulated a scenario in which our web server experienced a sudden surge in traffic, with 14000 concurrent user requests hitting our server simultaneously.

## Observations

### Initial Scenario :

**Connectivity:** 
- Users connected: 13,942
- Users timed out: 58
- Approximately 58 users experienced errors such as:
    -503 Service Unavailable
    -500 Internal Server Error

**Key Findings:**

- Network Traffic was observered under the simulated high load conditions.
- Network Traffic went from a resting 3.0 kib/s (Kibibits per second) to a 1.2 mib/s (Mebibits per second) this means that there has been a significant increase in the speed at which data is being transferred. Specifically, the data transfer rate has increased by a factor of 400.
  ![image](Blitz-2-images/Network-traffic.png)
  
- High CPU usage was observed under the simulated high load conditions.
- CPU reached 99.7% while the resting usage is 1.9% the drastic usage in cpu consumption can be attributed to the increased processing load caused by the high data transfer rates seen above. The CPU has to handle tasks like packet processing, data encryption/decryption and routing.
  ![image](Blitz-2-images/CPU-usage.png)
- 
- Regular Memory usage was observered under the simulared high load conditions.
- Memory usage maintained between the range on .7gb to 2.8gb both values well below half usage of the total 8gb.  
  ![image](Blitz-2-images/Memory-usage.png)
-
