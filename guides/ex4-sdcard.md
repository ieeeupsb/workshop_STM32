# SD Card

Storing and reading data from an sd card can be handy to generate log files or storing images. This microcontroller, like many other ARM microcontrollers have a middleware called FATFS that makes the communication between the STM32 and FAT filesystems easier.

## Exercise

We have a SD Card reader and you can use it to store temperature and humidity data that for this purpose can be generated randomly, without the sensor. We suggest you look at this examples code and write to the SD Card

Example library: https://github.com/G-Pereira/Electric-FIAT/blob/master/firmware/Core/Src/sd_wr.c

[Main Menu](../README.md) | [Next](ex5-lcd.md)