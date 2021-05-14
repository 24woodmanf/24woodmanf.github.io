# Finn


# Code (python) that allows ev3 sculpture to move based on a touch sensor 

ev3 = EV3Brick()

ev3.speaker.beep()

MotorR = Motor(Port.A)
MotorL = Motor(Port.B)
ts = TouchSensor(Port.S1)

while True:
    if ts.pressed():
        MotorR.run(2000)
        MotorL.run(2000)
        wait(200)
        MotorL.brake()
        MotorR.brake() 
    else:
        wait(2000)

       
 
