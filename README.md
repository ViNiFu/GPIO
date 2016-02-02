# GPIO
Raspberry Pi Universal GPIO Control for Delphi and FreePascal

# Dependencies
There are none.

# Building FreePascal for Raspberry Pi
You can build FreePascal and Lazarus for Raspberry Pi 2 using [this guide](http://otapi.com/2015/02/10/raspberry-pi-2-freepascal-lazarus-and-delphi/)

# How this library works
This library provides a "universal interface" for the Raspberry Pi's GPIO interface.

On the Raspberry Pi itself, commands and hooks passed to the GPIO interface are communicated directly to/from the physical GPIO interface of the Raspberry Pi itself.

If you're prototyping a solution using either FreePascal or Delphi on any other platform (Windows, Mac, iOS, Android, Linux), you are presented with a "software emulation" representing the Raspberry Pi's GPIO interface.

This enables you to convieniently build Raspberry Pi solutions on any platform using either Delphi or (more likely) FreePascal, then simply recompile on the Raspberry Pi itself, or cross-compile for the Raspberry Pi from another platform.

**Note that the emulation interface is only compiled into your binary by default on any non-Pi device.**

# Copyright and License
This library is produced by the unincorporated group known as "LaKraven Studios", by multiple developers originating with Simon J Stuart.

It is *loosely* based on the "PiGpio.pas" unit by Gabor Szollosi, but has been entirely rewritten from the ground-up. The original unit was used solely for a point of reference (to save some of the learning curve). Note that, at the time of publishing this repository on GitHub, "PiGpio.pas" has not been updated since 2013, and does not support the Raspberry Pi 2 GPIO interfaces. Our version supports *both*.

You are granted non-exclusive, world-wide rights to use and modify this unit as you see fit. You do not need to distribute your modifications (though you are encouraged to contribute improvements and bug fixes to this repository if you feel so-inclined).

You use this library entirely at your own risk, without guarantee or warranty of any kind (explicitly or implicitly). Nobody involved or associated with the production and/or maintenance of this library may be held responsible for losses and/or damages of any kind. Put simply "don't blame us!"
