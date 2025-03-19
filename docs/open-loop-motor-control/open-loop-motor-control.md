## Report goes here
**Aim**  
To make a buggy drive in a straight line and then edit the code for it to move at three different speeds, then calculate it's speed in meters per second.

**Method**  
With reference to the online material posted on canvas, the corresponding pins on the buggy were wired up. code was then uploaded to the ATMega328P MCU mounted on the buggy. When the buggy was turned on, the wheels did begin turn, allowing the buggy to move. However initially the buggy would veer quite heavily to the left whilst the motor parameters were identical. A few attempts were then made to make sure the buggy would drive in a straight line. This was done by increasing the speed of the left wheel to compensate for the bend to the left. Once the buggy was driving straight, different speeds for both wheels were implemented into the code. For each of the new wheel speeds, the time it took for the buggy to travel one meter was recorded. Then simple v=d/t was used to calculate the velocity of the buggy.

**Results**  
The first speed values recorded where:  
> #define MOTOR_L_PWM_INITIAL_VALUE 240  
> #define MOTOR_R_PWM_INITIAL_VALUE 200  

This took 3.49 seconds to travel one meter.

The second speed values recorded where:  
> #define MOTOR_L_PWM_INITIAL_VALUE 125  
> #define MOTOR_R_PWM_INITIAL_VALUE 100  

This took 6.43 seconds to travel one meter.

The third speed values recorded where:  
> #define MOTOR_L_PWM_INITIAL_VALUE 185  
> #define MOTOR_R_PWM_INITIAL_VALUE 150  

This took 3.91 seconds to travel one meter.


|Speed No.|Value|Time|Meters Per Second|
|--------|-------|-------|-------|
|1| L:240 R:200|3.49s|0.286 m/s|
|2| L:125 R:100|6.43s|0.155 m/s|
|3| L:185 R:150|3.91s|0.255 m/s|
