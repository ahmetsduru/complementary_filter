# Quadcopter Attitude Estimation using Complementary Filter

This repository contains an implementation of a complementary filter for realtime attitude estimation on a quadcopter platform. The filter utilizes data from accelerometer, gyroscope, and magnetometer sensors onboard a Mini Pixhawk flight controller. 

## Sensors and Data Frequency
- **Accelerometer**: Measures linear acceleration in three axes.
- **Gyroscope**: Measures angular velocity around three axes.
- **Magnetometer**: Provides orientation relative to the Earth's magnetic field.

All sensor data is sampled at a frequency of 20 Hz.

## Implementation Details
The complementary filter algorithm fuses accelerometer-magnetometer and gyroscope data to obtain a robust attitude estimation that is relatively immune to the drift inherent in all sensors.

## Usage
To use this code:
1. Clone the repository: `git clone https://github.com/ahmetsduru/complementary_filter.git`
2. Open the project in your preferred IDE or text editor.
3. Upload sensor data (`sensor_data.txt`) obtained from your Mini Pixhawk or use the provided sample data.
4. Compile and run `main.cpp` to observe the attitude estimation output.

## Dependencies
This project requires a C++ compiler that supports C++11 or later.

## License
This project is licensed under the MIT License.

## Acknowledgments
- The complementary filter implementation was inspired by [source/[link](https://ahrs.readthedocs.io/en/latest/filters/complementary.html)/reference].
