
# Nuttx Accelerometer Sensor Read
Simple accelerometer reading using NuttX tasks and queues.
## Requirements
MPU6050 driver, bind to /dev/i2c0.

## Executing

This was tested on Tiva-C TM4C1294-XL evaluation kit.
Clone this folder inside your examples folder and it should be good to go as an application.

```
cd ~/nuttxspace/apps/examples
git clone https://github.com/fdcavalcanti/real-time-sensor
cd ~/nuttxspace/nuttx
./tools/configure.sh tm4c1294-launchpad:nsh
```

## Example

```shell
nsh> sensor_read 
Starting Accelerometer Task Example
Opening message queue channel
Starting accelerometer task
Starting offload task
1 1.041 0.008 -0.038 
2 1.050 0.014 -0.047 
3 1.060 0.007 -0.054 
4 1.051 0.013 -0.043 
5 1.058 0.006 -0.052 
6 1.056 0.008 -0.051 
7 1.046 0.004 -0.051 
8 1.050 0.005 -0.065 
```

