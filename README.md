# Open Source Hand Tracking Live2D Model
A basic Live2D model which is rigged for arm and hand tracking. 

This model is open source the model and any parts of it can be used, copied and edited. No credit is necessary.

<img src="https://github.com/BluePengcho/Open_Source_Hand_Tracking_Live2D_Model/blob/main/Reference_Images/Skeleton.png" width="40%" height="40%">


This is not intended to be a guide on how to rig/model hands for Live2D but more for experimentation with motion tracking and Live2D.

If you are looking for a guide on hand rigging I recommend :-

* [[HOW TO: Live2d] Hands tracking for Vtube Studio](https://www.youtube.com/watch?v=oqdIBafz6i8) guide on YouTube by YoshinoArt 


If you are looking for software to use hand tracking with VTubeStudio I recommend checking out:-

* **Leap Motion To VTube Studio** by LuaLucky for use with a Leap Motion Controller 
    * [Source Code](https://github.com/lualucky/LeapMotionToVTubeStudio) and [Alpha Version](https://lualucky.itch.io/leapmotion-to-vtube-studio-plugin) (only hand tracking) 

* [VTubeStudio's built in hand tracking](https://github.com/DenchiSoft/VTubeStudio/wiki/Hand-Tracking) (only hand tracking)  

**For use with VTubeStudio**
------
* For convenience download and extract the **Skeleton_Model.zip** file   
* Copy/place the Skeleton_Model folder into the Live2DModels VTubeStudio folder:-
   *  <VTubeStudio.exe-Path>\VTube Studio_Data\StreamingAssets\Live2DModels (for Windows) 
   
* The output value parameter values might need to be changed in VTubeStudio, please see the parameter values tables below for the values to use.  
   
* The model also has the following extra custom parameters not used by default in VTubeStudio, an external VTubeStudio plugin is needed to use them:-
   * LeftUpperArmRotation
   * LeftForearmRotation
   * LeftUpperArmExtend
   * LeftForearmExtend
   * RightUpperArmRotation
   * RightForearmRotation
   * RightUpperArmExtend
   * RightForearmExtend
   
 * For the following parameters in VTubeStudio the **Smoothing Value** will need to be set to Zero:-
   * HandRightAngleX
   * HandLeftAngleX
   * RightForearmRotation
   * LeftForearmRotation

   This is necessary as VTubeStudio smoothes between a linear range e.g. 0 to 360 instead of a looping range which results in the parameters values quickly jumping back on itself and a consequent jerky motion, recommend adding smoothing code to any external VTubeStudio plugin for these parameters.  



**Notes**
------

* This model has only 30 parameters and should open with Live2D Cubism Editor Free Version 
* This model is rigged with arms and hands movement only, it does not have any other movement or facial expression rigging
* Hands are only rigged with the Hand AngleX and Hand AngleZ movement. There is no Hand AngleY movement (plan to add this to future versions once I can  find/figure out how)
* The hand rigging is very scuffed and was very much a learning experience. The methods used are probably not best practice. 
* Future versions plan to improve and rework the hand rigging for greater range of movement and finger positioning     

**Parameter Reference Images**
------
Please use these images for reference of the motions and relevant parameter values 

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
