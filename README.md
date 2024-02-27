<div align="center">

# Raspberry Pi Pico BNO055 IMU Driver

BNO055 IMU driver for raspberry pi pico (pico c/c++ sdk projects).
this code libraray developed as part of my main project "FCP" (autonomous flight controller project),
it can be used for other projects thats need imu sensor roll, pitch and yaw data.
based on the Bosch BNO055 chip (specifically Adafruit BNO055 sensor board).

Hardware:

[Raspberry Pi Pico](https://www.raspberrypi.com/products/raspberry-pi-pico/) •
[Adafruit BNO055](https://learn.adafruit.com/adafruit-bno055-absolute-orientation-sensor/overview)

</div>

<div>

# Example Of Use

```c++
IMUdriver imu_sensor;
IMUdata imu_container;
imu_sensor.IMUdriver::clear_container(imu_container);
imu_sensor.read_data(imu_container);
std::cout << "Roll: " << imu_sensor.roll << ", Pitch: " << imu_sensor.pitch << ", Yaw: " << imu_sensor.yaw << "." << std::endl;
```

</div>
