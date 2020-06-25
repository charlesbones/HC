# My sketch seems to upload successfully but does nothing

This behaviour can happen due to multiple reasons, in this article we will cover the most common possibilities and what to check .

## Option 1: Power supply

Check that the power supply is **stable** without any noisy signals and that the **current and voltage are enough** to power the board and any extra components connected to it.

## Option 2: `While (!Serial)`
Many of the IDE examples include a line with `while(!Serial)` in the `setup()` function of the sketch.
This line stops the sketch until the serial communication (usually between computer and board) on the selected serial port is ready.
This might give the impression that the sketch is not working since the program gets stuck in the "waiting for the communication to be ready" loop and it never reaches the main `loop()`.

If you don’t plan on using the communication, you can just comment or delete said line of code.

This feature applies on most of the Arduino products except:
* Arduino UNO
* Arduino Nano

# Option 3: Circuit
Make sure that the components connected to the board are working properly and there are no short circuits that might reset the board. Our recommendation is to test one component at time and slowly increase the amount of components connected to the board.
