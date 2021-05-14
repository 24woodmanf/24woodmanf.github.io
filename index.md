# Finn


# Code (python) that allows ev3 sculpture to move based on a touch sensor 

# #!/usr/bin/env pybricks-micropython
# from pybricks.hubs import EV3Brick
# from pybricks.ev3devices import (Motor, TouchSensor, ColorSensor,
# InfraredSensor, UltrasonicSensor, GyroSensor)
# from pybricks.parameters import Port, Stop, Direction, Button, Color
# from pybricks.tools import wait, StopWatch, DataLog
# from pybricks.robotics import DriveBase
# from pybricks.media.ev3dev import SoundFile, ImageFile


# This program requires LEGO EV3 MicroPython v2.0 or higher.
# Click "Open user guide" on the EV3 extension tab for more information.


# Create your objects here.
# ev3 = EV3Brick()


# Write your program here.
# ev3.speaker.beep()

# MotorR = Motor(Port.A)
# MotorL = Motor(Port.B)
# ts = TouchSensor(Port.S1)

# while True:
    if ts.pressed():
        MotorR.run(2000)
        MotorL.run(2000)
        wait(200)
        MotorL.brake()
        MotorR.brake() 
    else:
        wait(2000)

 
 


 
