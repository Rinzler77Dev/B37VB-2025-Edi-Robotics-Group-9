## Report goes here
**Aim**
To make a buggy drive in a straight line and then edit the code for it to move at three different speeds, then calculate it's speed in meters per second.

**Method**
With reference to the online material posted on canvas, the corresponding pins on the buggy were wired up. code was then uploaded to the ATMega328P MCU mounted on the buggy. When the buggy was turned on, the wheels did begin turn, allowing the buggy to move. However initially the buggy would veer quite heavily to the left. a few attempts were made to make sure the buggy would drive in a straight line. This was done by increasing the speed of the left wheel. Once the buggy was funcioning normally, different speeds for both wheels were implemented into the code. For each of the new wheel speeds, the time it took for the buggy to travel one meter was recorded. Then simple v=d/t was used to calculate the velocity of the buggy.

default code veers left
balancing changes: L motor > 255 (max) too much > 220 too little > 235 almost > 240 almost again > robert reccommends reducing R wheel > 190 major fail too much right > 195 || 240 L 200 R
different speeds: 120 100 halfing now veers left > 160 100 too much going right > 140 X > 125 100 works very well at half speed
different speed 2: 175 150 no worky / wonky > 180 > 185 (L) works good / perfect!

Speed 1:  (240 200): 3.49s to go 1m
Speed 2: (125 100): 6.43s to go 1m
Speed 3 (185 150): 3.91s to go 1m 

|Speed No.|Value|Time|Meters Per Second|
|--------|-------|-------|-------|
|1| L:240 R:200|3.49s|0.286 m/s|
|2| L:125 R:100|6.43s|0.155 m/s|
|3| L:185 R:150|3.91s|0.255 m/s|
