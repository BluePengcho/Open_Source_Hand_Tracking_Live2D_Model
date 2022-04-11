# Open Source Hand Tracking Live2D Model
A basic live2D model which is rigged for arm and hand tracking. 

This model is open source, the model and any parts of it can be used, copied and edited however you wish. No credit is necessary.

<img src="https://github.com/BluePengcho/Open_Source_Hand_Tracking_Live2D_Model/blob/main/Reference_Images/Skeleton.png" width="40%" height="40%">


This is not inteded to be a guide on how to rig/model hands for Live2D but more for expermintation with motion tracking and Live2D.

If you are looking for a guide on hand riging I recomend :-

* [[HOW TO: Live2d] Hands tracking for Vtube Studio](https://www.youtube.com/watch?v=oqdIBafz6i8) Youtube guide by YoshinoArt 


If you are looking for software to use hand tracking with VtubeStudio I recomend checking out:-

* **Leap Motion To VTube Studio** by LuaLucky for use with a Leap Motion Controller 
    * [Source Code](https://github.com/lualucky/LeapMotionToVTubeStudio) (arm and hand tracking) 
    * [Alpha Version](https://lualucky.itch.io/leapmotion-to-vtube-studio-plugin) (only hand tracking) 

* [VtubeStudios built in hand tracking](https://github.com/DenchiSoft/VTubeStudio/wiki/Hand-Tracking) (only hand tracking)  


Notes:-

* This model has only 30 Paramaters and should be able to be opened with Live2D Cubism Editor Free Version 
* This model is rigged with arms and hands movement only, it does not have any other movment or facial expresion rigging
* Hands are only rigged with the Hand AngleX and Hand AngleZ movement. There is no Hand AngleY movement (plan to add this to future version once I can  find/figure out how)

* To use the model in VtubeStudio please copy the Skell_Model folder into the VtubeStudio folder:-
   *  <VtubeStudio.exe-Path>\VTube Studio_Data\StreamingAssets\Live2DModels (for Windows) 
   
* The output value paramater values will need to be change in VtubeStudio (please see the Parameter Values tables bellow for the values to use)  
   
* For the folowing peramaters an external VtubeStudio pluggin will need to create the custome paramters for use within VtubeStudio:-
   * LeftUpperArmRotation
   * LeftForearmRotation
   * LeftUpperArmExtend
   * LeftForearmExtend
   * RightUpperArmRotation
   * RightForearmRotation
   * RightUpperArmExtend
   * RightForearmExtend
   
 * For the folowing peramaters in VtubeStudio the Smoothing Value will need to be set to Zero:-
   * HandRightAngleX
   * HandLeftAngleX
   * RightForearmRotation
   * LeftForearmRotation

   This is necessary as VTubeStudio smoothes between a linear range e.g. 0 to 360 instead of a looping range which results in the peramaters values quicky jumping back on itself and consequently a jerky motion, recommend adding smoothing code to any extenal plugins for these peramaters.  
   
* The hand rigging is very skuffed and was very much a learning experiance. The methods used are probably not best practice. 
* For future version plan to rework the hand rigging for greater range of movement and finger positioning     

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
