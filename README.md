# Open Source Hand Tracking Live2D Model
An open source live2D basic model rigged for arm and hand tracking

<img src="https://github.com/BluePengcho/Open_Source_Hand_Tracking_Live2D_Model/blob/main/Reference_Images/Skeleton.png" width="40%" height="40%">


This is not inteded to be a guide on how to rig/model hands for Live2D but more for expermintation with motion tracking and Live2D.

If you are looking for a guide on hand riging I recomend :-

* [[HOW TO: Live2d] Hands tracking for Vtube Studio](https://www.youtube.com/watch?v=oqdIBafz6i8) Youtube guide by YoshinoArt 


If you are looking for software to use hand tracking with VtubeStudio I recomend checking out:-

* **Leap Motion To VTube Studio** by LuaLucky for use with a Leap Motion Controller 
    * [Source Code](https://github.com/lualucky/LeapMotionToVTubeStudio) (arm and hand tracking) 
    * [Alpha Version](https://lualucky.itch.io/leapmotion-to-vtube-studio-plugin) (only hand tracking) 

* [VtubeStudios built in hand tracking](https://github.com/DenchiSoft/VTubeStudio/wiki/Hand-Tracking) (only hand tracking)  


**Parameter Reference Images**
------

<img src="https://github.com/BluePengcho/Open_Source_Hand_Tracking_Live2D_Model/blob/main/Reference_Images/Live2D_Upper_Arm_Rotation.png" width="40%" height="40%">

<img src="https://github.com/BluePengcho/Open_Source_Hand_Tracking_Live2D_Model/blob/main/Reference_Images/Live2D_Forearm_Rotation.png" width="40%" height="40%">

<img src="https://github.com/BluePengcho/Open_Source_Hand_Tracking_Live2D_Model/blob/main/Reference_Images/Live2d_Upper_Arm_Extension.png" width="40%" height="40%">

<img src="https://github.com/BluePengcho/Open_Source_Hand_Tracking_Live2D_Model/blob/main/Reference_Images/Live2D_Forearm_Extension.png" width="40%" height="40%">

<img src="https://github.com/BluePengcho/Open_Source_Hand_Tracking_Live2D_Model/blob/main/Reference_Images/Live2D_Hand_Rotation_AngleX.png" width="40%" height="40%">

<img src="https://github.com/BluePengcho/Open_Source_Hand_Tracking_Live2D_Model/blob/main/Reference_Images/Live2D_Hand_Rotation_AngleZ.png" width="40%" height="40%">

<img src="https://github.com/BluePengcho/Open_Source_Hand_Tracking_Live2D_Model/blob/main/Reference_Images/Live2D_Finger_Rotation.png" width="40%" height="40%">

**Left Arm Parameter Values**
------
|         | Minimum            | Default   |Maximum   |
| ------------- |:-------------:| -----:| -----:|
|HandLeftAngleX|             -60|  0| 60|
|HandLeftAngleZ|             -90|  0| 90|
|HandLeftFinger_1_Thumb|       0|  1|  1|
|HandLeftFinger_2_Index |      0|  1|  1|
|HandLeftFinger_3_Middle|      0|  1|  1|
|HandLeftFinger_4_Ring |       0|  1|  1|
|HandLeftFinger_5_Pinky|       0|  1|  1|
|HandLeftRotation_2_Index |   -1|  0|  1|
|HandLeftRotation_3_Middle|   -1|  0|  1|
|HandLeftRotation_4_Ring |    -1|  0|  1|
|HandLeftRotation_5_Pinky|    -1|  0|  1|
|LeftUpperArmRotation|       -30|  0| 30|
|LeftForearmRotation |       -30|  0| 30|
|LeftUpperArmExtend |          0|  0| 30|
|LeftForearmExtend |           0|  0| 30|

**Right Arm Parameter Values**
------

|         | Minimum            | Default   |Maximum   |
| ------------- |:-------------:| -----:| -----:|
|HandRightAngleX|             -60|  0| 60|
|HandRightAngleZ|             -90|  0| 90|
|HandRightFinger_1_Thumb|       0|  1|  1|
|HandRightFinger_2_Index |      0|  1|  1|
|HandRightFinger_3_Middle|      0|  1|  1|
|HandRightFinger_4_Ring |       0|  1|  1|
|HandRightFinger_5_Pinky|       0|  1|  1|
|HandRightRotation_2_Index |   -1|  0|  1|
|HandRightRotation_3_Middle|   -1|  0|  1|
|HandRightRotation_4_Ring |    -1|  0|  1|
|HandRightRotation_5_Pinky|    -1|  0|  1|
|RightUpperArmRotation|       -30|  0| 30|
|RightForearmRotation |       -30|  0| 30|
|RightUpperArmExtend |          0|  0| 30|
|RightForearmExtend |           0|  0| 30|
