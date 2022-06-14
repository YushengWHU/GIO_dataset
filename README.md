# GIO_dataset
This repository shares some datasets for general lightweight odometry. *A General Lightweight Odometry Frameworkfor Intelligent Vehicles*</br>
The first sequence is for HQ-1 IV, composed of 4 calibrated LiDARs (2 Leishen CH32, 2 RS-Bperal), 7 surround view cameras, GNSS, IMU, and chassis info. Topics info: </br>
```C++
/athena/mdc/RadarListInfo                
/cam_front_center/csi_cam/image_raw/compressed             
/cam_front_left/csi_cam/image_raw/compressed                  
/cam_front_right/csi_cam/image_raw/compressed
/cam_left_back/csi_cam/image_raw/compressed
/cam_left_front/csi_cam/image_raw/compressed
/cam_right_back/csi_cam/image_raw/compressed
/cam_right_front/csi_cam/image_raw/compressed
/chassis
/gnssImu
/lidar1/points_raw
/lidar2/points_raw
/lidar3/points_raw
/lidar4/points_raw
```
Specifically, the /chassis info is: </br>
```C++
Header header                            #header
float32 wheel_speed_fr                   #front right wheel speed     kph
float32 wheel_speed_fl                   #front left wheel speed      kph
float32 wheel_speed_rr                   #rear right wheel speed      kph
float32 wheel_speed_rl                   #rear left wheel speed       kph
#float32 velocity                        #linear velocity
```
and the /gnssImu is: </br>
```C++
Header header                           
float64 longitude                       
float64 latitude                       
float64 elevation                       
geometry_msgs/Point utmPosition         
int32 utmZoneNum                        
uint8 utmZoneChar                       
geometry_msgs/Point attitude            
geometry_msgs/Point linearVelocity     
geometry_msgs/Point sdPosition          
geometry_msgs/Point sdVelocity          
geometry_msgs/Point sdAttitude          
float64 cep68                           
float64 cep95                           
float64 second                          
int32 satUseNum                         
int32 satInViewNum                      
uint16 solutionStatus                  
uint16 positionType                    
float32 pDop                            
float32 hDop                            
float32 vDop                            
geometry_msgs/Point attitudeDual       
geometry_msgs/Point sdAngleDual        
float64 baseLineLengthDual              
int32 solutionStatusDual                
int32 positionTypeDual                 
int32 solutionSourceDual                
uint32 aoc                             
uint32 rtkBaseline                      
geometry_msgs/Point angularVelocity     
geometry_msgs/Point acceleration        
```
For chinese friends, the link is: 链接：https://pan.baidu.com/s/1aeKO_O52zrpVCi1Zf5TcZQ 提取码：1234 </br>
