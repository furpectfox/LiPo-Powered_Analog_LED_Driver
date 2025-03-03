# Lipo-Powered Analog LED Driver (on-going project)
This circuit uses only ICs and discrete components to control the dimming of an LED bar. No microcontroller is involved.

## Features:

### Voltage Doubler:
The circuit incorporates a voltage multiplier that boosts the LiPo battery voltage to nearly twice its original level. This ensures the voltage driving the N-channel MOSFET gate is higher than the gate-source threshold voltage, even as the battery voltage decreases over time.

### PWM Generator:
An LM339 Voltage Comparator is used to generate a square wave. The square wave is then converted into a semi-ramp waveform and fed to a second voltage comparator to be compared with a variable DC voltage. The output is a square wave with a controllable duty cycle, which drives the MOSFET gate.

This circuit has a resistor selector circuit, allowing the user to switch between three duty cycles and thus modes of brightness.
So why not use a potentiometer, which would allow any level of dimming and simplify the circuit greatly, since the resistor selector part is not needed? The answer is simple, I want to learn to use a variety of ICs and different ways to do the same thing.

### Duty Cycle Selector
The circuit includes a resistor selector, allowing the user to switch between three preset duty cycles, thus providing different brightness modes.

Why not use a potentiometer?
While a potentiometer would simplify the design and provide continuous dimming control, I opted to use the resistor selector for two main reasons:
1. Learning Experience: I wanted to explore a variety of ICs and different circuit design methods to achieve the same functionality.
2. Component Variety: This approach gives me hands-on experience with multiple ICs and provides an interesting challenge for learning circuit design techniques.

## Prototype
![prototype](images/prototype.jpg)
![breadboard_test](images/breadboard_test.gif)