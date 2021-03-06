# Odroid Testing

## Equipment

 * Lipo battery
 * Power board (tested with a working buzzer)
 * Odroid
 * Power board on|off loop
 * Odroid power cable
 * Micro USB cable
 * USB stick (with the following code in a robot.zip from the IDE):
    ``` python
    import time
    from sr.robot import *
    R = Robot()

    while True:
        R.power.beep(200, note='a')
        time.sleep(0.6)
    ```

## Procedure

*Execution time*: 1 minutes per board.

 1. Assemble minimal kit
 2. Insert USB stick into Odroid
 3. Turn on power board
 4. Wait for the start LED to flash
 5. Press the start button
 6. The power board should beep. If it does the Odroid is a pass, otherwise it is a fail.
