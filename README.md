#ServoTimer2
===========

ServoTimer2 is a simple servo library for Arduino 1.x that does not use Timer1 in case of a conflict.

Original (c) 2008 Michael Margolis, updated for Arduino 1.x and example added by Nick Bontrager 2013.

##Notes
write takes a value of microseconds, 1000 for all the way left, 1500 for center, 2000 for all the way right.

##API
===========
The methods are:
   ServoTimer2 - Class for manipulating servo motors connected to Arduino pins.
   attach(pin )  - Attaches a servo motor to an i/o pin.
   attach(pin, min, max  ) - Attaches to a pin setting min and max values in microseconds
    default min is 544, max is 2400  
 
   write()     - Sets the servo pulse width in microseconds.
   read()      - Gets the last written servo pulse width in microseconds. 
   attached()  - Returns true if there is a servo attached. 
   detach()    - Stops an attached servos from pulsing its i/o pin. 
