# Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
```
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
  pos=[[1,30],[2,40],[3,90]]
  robot = getRobot()
  robot.driveJoints(0,0,0,0,0,0)
  delay(5)
  for i in pos:
    robot.Controller.moveJoint(i[0],i[1])
    delay(5)

```
## Output
### 1. Generic Articulated Robot
![image](https://github.com/Udhayasankaran04/Movement-of-Robot-Joints/assets/119393933/cf2f46f2-23f8-4d78-912a-96adcb9113e6)

### 2. robot.driveJoints(0,0,0,0,0,0)
![image](https://github.com/Udhayasankaran04/Movement-of-Robot-Joints/assets/119393933/47210e6b-5d70-4f04-bb4f-9b2f60b24e47)

### 3. Movement of Joint1
![image](https://github.com/Udhayasankaran04/Movement-of-Robot-Joints/assets/119393933/77289b1c-0e76-4d84-ac1d-0154ed3c2a9d)

### 3. Movement of Joint2
![image](https://github.com/Udhayasankaran04/Movement-of-Robot-Joints/assets/119393933/810a803b-7872-4cef-853f-78503e03b9ec)

### 3. Movement of Joint3
![image](https://github.com/Udhayasankaran04/Movement-of-Robot-Joints/assets/119393933/31e2b94c-7f96-4fae-add0-0bc40559bb07)

## Result 
Thus the different robots joints are moved with the help of python list.


