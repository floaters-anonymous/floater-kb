FAQ
===

### VESC

  * How to create csv logs in VESC
    ((https://pev.dev/t/how-to-create-csv-logs/436))


### VESC Terminal functions

  * show hall sensor raw data
    ```c
    Hall_analyze 10
    ```

#### CAN interfaces:

  * multiple can interfaces
    > I work with CAN in lots of OTHER applications that being said when you have more than 2 devices you need to assign which are the terminators (120 ohm resistors) hope this helps


#### Hall Sensors:

  * testing sensors ((https://youtu.be/5WpwJNKCEnY))
    > figure out/trace the 5v/ground/signal, then power the 5v and ground via bench power supply 
    > move the motor through its poles (slowly spin the motor)
    > Hall effect sensors move between two voltage values (0 and 5v).
    > Multimeter should report voltages from 0v to 5v


