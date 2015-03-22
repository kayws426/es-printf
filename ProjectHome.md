# Printf for Embedded Systems #

The standard 'C' printf function and its derivatives can be extremely useful, but in a resource-constrained embedded system it is often just too big. Whilst some compilers provide an integer-only version to reduce bloat, this version is highly configurable so you can trim away all the bells and whistles you don't actually use to reduce it to minimal size.

Sending your output to a serial port (or any other interface) is as easy as providing a function to write a character to that port.

The functions provided by your compiler are often not thread-safe either, using static buffers to do some of the formatting. This version uses no static buffers, making it suitable for RTOS-based systems.

The original target for this function was the 8-bit AVR family with the WinAVR GCC compiler.