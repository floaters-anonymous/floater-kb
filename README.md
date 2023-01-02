![BalanceBoard](https://gitlab.com/uploads/-/system/project/avatar/41185754/onewheel_xr.jpg)
# floaters-anonymous
## floating knowledge base / resources

### Reference:

* [1wheel on Gitbook.io](https://app.gitbook.com/invite/CAI2PvcEBO6EQLwSDjOW/N7ftWtxnJP35ZuZ7ps1O)
* [esk8_diy-onewheel-hoverboard](https://forum.esk8.news/t/diy-onewheel-hoverboard/18862)


### VESC terminal reference

* show hall sensor raw data
  ```c
  Hall_analyze 10
  ```

## Troubleshooting

#### CAN interfaces:

  * multiple can interfaces
    > I work with CAN in lots of OTHER applications that being said when you have more than 2 devices you need to assign which are the terminators (120 ohm resistors) hope this helps

#### Hall Sensors:

  * testing sensors ((https://youtu.be/5WpwJNKCEnY))
    > If you are comfortable, you could figure out/trace the 5v/ground/signal, then power the 5v and ground via bench power supply (or try to use the focer at the same time and just DMM the signal?) and move the motor through its poles (slowly spin the motor). It should go from 0v to 5v since Hall effect sensors move between two voltage values (0 and 5v).



### Other Links
* (https://pev.dev/t/faq-batteries-wiki/92)
* (https://pev.dev/t/vesc-xr-step-by-step-conversion-guide/105)
* (https://pev.dev/t/connecting-to-pc-vesc-tool-with-bluetooth-how-to/291)
* (https://pev.dev/t/guide-how-to-wire-fm-bms-as-charge-only-for-your-vesc/322/3)
* (https://pev.dev/t/bluetooth-module-wiring-diagram-nrf51822/137)
* (https://pev.dev/t/how-to-guides-for-basic-tasks/341)
* (https://pev.dev/t/flash-vesc-bootloader-firmware-with-st-link/453)
* (https://customwheel.shop/blog/manual-how-to-install-your-controller)


## License
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.
