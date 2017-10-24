# Omega2 Libraries and Headers

This repository contains header (.h) and shared library objects (.so) files for common library needed during Omega2 C development.

I noticed that atleast during my developments, I could not link my programs against the library files which were installed / installable on the Omega2+. `gcc` would always through an `undefined reference to ...` error, although the library file was given to it. However, after compiling them on the Omega2+ or cross-compiling them locally, they would successfully link. I have thus created this repository of libraries and header files so that developers don't need to recompile these libs themselves. 

The following libraries are contained here:
	- libugpio ([from OpenWRT](https://dev.openwrt.org/export/35269/packages/libs/libugpio))
	- libonioni2c, libonionmcp23008, libonionoledexp, libonionpwmexp, libonionrelayexp, liboniondebug ([from OnionIoT](https://github.com/OnionIoT/i2c-exp-driver/))
	- libalsa (cross-compiled for Omega2(+) from alsa-lib-1.1.4.1.tar.bz2 at ftp://ftp.alsa-project.org/pub/lib/)
	- libonionspi ([from OnionIoT](https://github.com/OnionIoT/spi-gpio-driver))
	- libili9225 (my own library [here](https://github.com/gamer-cndg/omega2-ili9225))
	- libwiiclassic (my own library [here](https://github.com/gamer-cndg/omega2-wii-classic-controller/))

### Disclaimer

By no means am I claiming copyright on any of these libraries. As previously explained, the header files and compiled binaries are just here to ease development.