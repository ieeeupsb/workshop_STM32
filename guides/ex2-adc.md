# Analog to Digital Converter

Sampling an analog signal is a process that takes a lot of time. Because of this the STM32 has multiple ways to implement this.

- Processor asks for a convesion and waits for it
    - blocks execution
    - only acceptable for simple applications
- Processor asks for a conversion, does other things and an interruption occurs when conversion is complete
    - suitable for medium complexity applications
    - a mess if the application already has a lot of interruption routines.
    - STM32 handles this well by having a waiting list for interruptions, that ensures every interruptions is handled at some point.
- Processor asks for a conversion and tells the ADC controller and DMA interface where to store the result and nver worries about it again
    - Non blocking
    - Perfect for complex applications
    - If its important to know when a new value is present it can be similar to the previous method

## Exercise

Here it is examples for each mode we've described. Have a look and try to implement them.

https://github.com/cnoviello/mastering-stm32/tree/master/nucleo-f103RB/src/ch12

You can also tweak the advanced parameters on STM32CubeMX to change sampling priority between different channels, their sampling time and many other things.

[Main Menu](../README.md) | [Next](ex3-buses.md)