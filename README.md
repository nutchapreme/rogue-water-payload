# rogue-water-payload
Payload electronics for NYU's first hybrid rocket

# First prototype
**Components**: EasyMini, Arduino Nano, L298N, stepper motor, standard servo, 2X 9V Battery\

**How it works**: EasyMini detects altitude, once reach apogee it sends signal to Arduino to turn servo 90 degree pos, L298N drives the motor to push water-ballast\

**Issue**: payload was too messy, cannot adjust to higher speed without losing torque strength

# Cleaned up payload
**Component**: BMP390 module, Arduino Nano, A4988, stepper motor, standard servo, 2S Lipo
**How it works**: BMP390 detects change in pressure, once reach apogee it sends signal to Arduino to turn servo 90 degree pos, A4988 drives the motor to push water-ballast
**Improvement**: All the wires are soldered into a single protoboard, got the motor to spin a lot faster while remaining high torque

# PCB
**Component**: BMP388 (bare barometer), ATmega328P, bare DRV8434 chip, breakout pins for motors, XT30
Take all the bare components and keep the logic in the prototype
