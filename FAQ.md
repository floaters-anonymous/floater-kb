FAQ
===

### Batteries

  * [Battery Pack Primer Info](https://pev.dev/t/battery-pack-primer/366)

### VESC

  * How to create csv logs in VESC
    ((https://pev.dev/t/how-to-create-csv-logs/436))

  * IMU calibration - [excellent IMU calibration video](https://www.youtube.com/watch?v=vVvjHY5lFLs)
    * once IMU accel/gyro is setup and yaw offset is correct
      * LFOCer 3.0 - yaw offset == 0
      * LFOCer 3.1 - yaw offset == 90*
    * Pitch - positive values expected when "nose up/high"
    * Pitch - negative values expected when "nose down/low"
    * Corrections:
      * if pitch values are reversed, yaw offset needs to be offset by another 180*
      * Example: (for LFOC3.1) yaw offset should be changed to -90* or 270*

### VESC Terminal functions

  * show hall sensor raw data
    ```c
    Hall_analyze 10
    ```

#### CAN interfaces:

  * multiple can interfaces
    > I work with CAN in lots of OTHER applications that being said when you have more than 2 devices you need to assign which are the terminators (120 ohm resistors) hope this helps


#### Motor Hall Sensors:

  * [Motor Setup](https://pev.dev/t/how-to-configure-motor/486)
  * [What is a Hall Sensor?](https://ie.rs-online.com/web/generalDisplay.html?id=ideas-and-advice/hall-effect-sensors-guide)

  * testing sensors ((https://youtu.be/5WpwJNKCEnY))
    > figure out/trace the 5v/ground/signal, then power the 5v and ground via bench power supply
    > move the motor through its poles (slowly spin the motor)
    > Hall effect sensors move between two voltage values (0 and 5v).
    > Multimeter should report voltages from 0v to 5v

#### rESCue with NeoPixels

  * ![img: neopixel with rESCue](https://raw.githubusercontent.com/thankthemaker/rESCue/master/docs/images/neopixel-wiring.png)

#### XLR charge input connector

  * While XLR connecters are ubiquitous, the specific type that fits in the controller
    boxes available as STL files are these, made by [Neutrik - NC3MPR-HD](./Datasheets/NEUTRIK__XLR__NC3MPR.pdf)
  * This very specific connector seems to be consistently availabile from [Newark](https://www.newark.com/neutrik/nc3mpr-hd/xlr-audio-connector-plug-3-panel/dp/31M5702)
    see Newark product page, [item# 31M5702](https://www.newark.com/neutrik/nc3mpr-hd/xlr-audio-connector-plug-3-panel/dp/31M5702)

### XR Components
Official Specs (from [onewheel.wiki](onewheel.wiki))

  > MOTOR : 750W Hypercore hub motor
  > BATTERY : Nickel Manganese Cobalt Oxide (NMC) 324Wh 63V
  > SENSORS : Solid State MEMS 6-DOF
  > TIRE : 11.5×6.5-6 Vega
  > MAX LEAN ANGLE : >30 degrees
  > TOP SPEED : 19MPH / 30KPH
  > TYPICAL RANGE : 12-18 MI / 19-29 KM
  > DIMENSIONS : 9×11.5×30 (IN) / 23x29.21x72.6 (CM)
  > WEIGHT : 27 LB / 12.5 KG
  > RECHARGE TIME : 100 mins* (FY6303200 charger)


