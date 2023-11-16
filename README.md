# EXP-7 Movement-of-Robot-Joints
## Date: 7.11.1023
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
```python

from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
pos = [[1,30],[2,40],[3,90]]
robot = getRobot()
robot.driveJoints (0,0,0,0,0,0)
delay(5)
for i in pos:
robot.Controller.moveJoint (i[0],i[1])
delay (5)

```
## Output
### 1. Generic Articulated Robot

![image](https://github.com/Richard01072002/Movement-of-Robot-Joints/assets/141472248/ccdf324d-9e37-4566-9326-011fdf81ba63)


### 2. robot.driveJoints(0,0,0,0,0,0)

![image](https://github.com/Richard01072002/Movement-of-Robot-Joints/assets/141472248/8c7b7b74-8c35-4659-a08b-3598adf8547f)

### 3. Movement of Joint1

![image](https://github.com/Richard01072002/Movement-of-Robot-Joints/assets/141472248/7f24c97a-af60-4eff-b00b-ed2bfcb0fccc)


### 3. Movement of Joint2

![image](https://github.com/Richard01072002/Movement-of-Robot-Joints/assets/141472248/2f2cc0eb-31a0-4fa2-ba4d-61e8e85057b8)


### 3. Movement of Joint3

![image](https://github.com/Richard01072002/Movement-of-Robot-Joints/assets/141472248/4235c22a-6963-4dbc-b23f-9f4acd55469d)

## Result 
Thus the different robots joints are moved with the help of python list.


