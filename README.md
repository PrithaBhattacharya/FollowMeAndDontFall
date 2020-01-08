# FollowMeAndDontFall
This is a project to create a follow-me-bot using the best low-cost technology available. 

## Motivation Behind Project - 
We saw a video on YouTube and were fascinated by the concept of a suitcase following its owner around inside an airport while avoiding all obstacles coming in its way. Although such products are already available in the market, they are quite costly and we did not come across a lot of hobbyist projects in this domain. So we decided to explore the various low-cost hobbyist approaches to this concept in this project. 

## Initial Thoughts - 
When we first sat down to solve the problem, the basic outline we had in our mind was -
STEP1- Find a suitable sensor that can help us keep a track of the target person/object.
STEP2- Write a code to move our bot according to the sensor output so as to follow the target.

Expanding on STEP1, we came across many methods and various sensors to track the target person/object, some of which are described in somewhat detail in the next sub-section. 


## Exploring various Modules -  
### The nrf24l01 module- 
 For detailed information regarding this sensor, please refer to its datasheet at          https://www.sparkfun.com/datasheets/Components/nRF24L01_prelim_prod_spec_1_2.pdf
 
 **Pros** -
 * Transmitted signal can be recieved in fairly good strength across physical barriers like walls, or people moving around. Has a long      range of operation.
 
 **Cons** -
 * RSSI values cannot be calculated and thus it is difficult to compare the strengths of the signal at any random points.
 * The Antenna is omni-directional and does not conviniently give us a sense of direction from where the signal recieved is maximum. 
 
### The nrf51822 module-
  For detailed information regarding this sensor, please refer to its datasheet at 
  https://www.nordicsemi.com/-/media/Software-and-other-downloads/Product-Briefs/nRF51822-product-brief.pdf?la=en&hash=A4B5A9AA6675A58F7B779AF81C860CD69EB867FD
  
  **Pros**-
  * RSSI values can be easily detected and this can be further used to determine the distance between the bot and the target object.
  * Has BLE
  
  **Cons**-
  * The Antenna is omni-directional and does not conviniently give us a sense of direction from where the signal recieved is maximum.
  
### The hc-05 bluetooth module- 
  For detailed information regarding this sensor, please refer to its comprehensive guide at
  http://www.electronicaestudio.com/docs/istd016A.pdf
  
  **Pros**-
  * RSSI values can be detected. 
  * Uses bluetooth and thus eliminates the need of a transmittor-reciever pair. Our phones, or any blutooth enabled device can act as a     transmittor. 
  
  **Cons**-
  * The Antenna is omni-directional and does not conviniently give us a sense of direction from where the signal recieved is maximum.
  * Has a very short range of operation. 
  
### The GPS module- 

### OpenCV on Camera module of RPi-

## The Journey-
  *Problem1*- Finding the distance from the target and the direction of target's motion.

 
 
 


