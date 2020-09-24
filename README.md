# Autonomous-Vehicle-State-Estimator

This is the final project in the Course 2 - State Estimation and Localization for Self-Driving Cars of the Self-Driving Car Specialization offered by Coursera 

Note: According to Coursera's Honor Code none of the solutions can be shared in contrast to Udacity hence I am only sharing the results.

## Following section is an adapted version of the project rubric from Coursera

Part 1: First, we fill in the skeleton implementation of the ES-EKF that is provided, by writing code to perform the filter prediction step and the correction step. The filter relies on IMU data to propagate the state forward in time, and GPS and LIDAR position updates to correct the state estimate. For Part 1 of the project, the sensor data are prepackaged - it is possible to visualize the output of the estimator and compare it to the ground truth vehicle position (the ground truth position data are also provided). The complete filter implementation is tested by comparing the estimated vehicle position (produced by your code) with the ground truth position, for a 'hold out' portion of the trajectory (i.e., for which ground truth is not provided).

Part 2: Here, we examine the effects of sensor miscalibration on the vehicle pose estimates. Specifically, we will uncomment a block of code that intentionally alters the transformation between the LIDAR sensor frame and the IMU sensor frame; use of the incorrect transform will result in errors in the vehicle position estimates. After looking at the errors, our task is to determine how to adjust the filter parameters (noise variances) to attempt to compensate for these errors. The filter code itself should remain unchanged. Our updated filter (with the new parameter(s)) will be tested in the same way as in Part 1.

Part 3: Here, we will explore the effects of sensor dropout, that is, when all external positioning information (from GPS and LIDAR) is lost for a short period of time. For Part 3, you will load a different dataset where a portion of the GPS and LIDAR measurements are missing (see the detailed instructions below). The goal of Part 3 is to illustrate how the loss of external corrections results in drift in the vehicle position estimate, and also to aid in understanding how the uncertainty in the position estimate changes when sensor measurements are unavailable.

## Results

1. GroundTruth_xx.png - shows the ground truth trajectory for respective part in project in x, y, z co-ordinates in meters.
2. xx_result_analysis.png - shows the comparison of the ground truth and estimated trajectory for respective part in project in x, y, z co-ordinates in meters.
3. xx_error_plot.png - shows the error in the estimate compared to ground truth for the x, y, z co-ordinates (in meters) and roll, pitch, yaw (in radians).
