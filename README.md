# Data traces
The current repository contains real data traces from LiDAR (Robosense Helios 16) and Camera (Logitech C920 HD PRO) sensors which can be used to calibrate the Time-Sensitive Networking (TSN) simulation models. In particular, they serve as input for the simulation models presented in the paper "Cross-Validating Open Source In-Vehicle TSN Simulation Models with COTS Hardware Testebed", accepted for publication in the IEEE Vehicular Networking Conference (VNC 2024).

# License
© [2024] Luxembourg Institute of Science and Technology.
This work is licensed under a Creative Commons Attribution-ShareAlike 4.0 International License.

## Description
### PCAP files
Files containing a detailed network packet data. 

### CSV files
Each record in the ```.csv ```files is a tuple ```(Timestamp, FrameSize, InterFrameGap)```, which can be used to generate frames with variable sizes and inter-frame gaps in the simulation.

The ```Timestamp``` reprsents the time in seconds.

The ```FrameSize``` represents the size of the frame measured in *bits*.

The ```InterFrameGap``` represents the time differnece between two consecutive frames measured in seconds.

## Camera
#### Files:
- camera_datatrace.pcap  ```(IP.src == 192.168.4.5)```
- camera_datatrace.csv

## LiDAR
#### Files:
- lidar_datatrace.pcap ```(IP.src == 192.168.4.200)```
- lidar_datatrace.csv
