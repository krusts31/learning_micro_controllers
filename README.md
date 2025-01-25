# micro controllers

## RP2040

### HARDWARE

#### Procesor
2 cores
133 MHz

#### Memmory
264KB

6 banks of 264 KB. Each bank can be used independetly.

are these banks used to store code? 
are theye used for malloc?

#### PIO(programmable Input output)
supports uncommon comunication protocols that maybe wear not intended to work with the microcontroller at manufacturing.

#### Dedicated hardeware for commun protocols

I2C, SPI< UAER and other have dedicated hardware blocks.

#### DEDICATED I/O for SPI flash(supporing XIP)

##### SPI flash
RP2040 does not have onboard falsh for prgoram storag, so it relies on ternal SPI flash memmory.
what does this mean?

##### Dedicated I/O for SPI flash

6pins are specifically reserved for high-speed communication with the flash memory, ensuring efficient execution.

##### XIP(eXecute In Place)
Allows for executing of code stored in SPI flash without copying it into SRAM first.
Saves sram and speed up execution.

##### 30 GPIO pins

what is `ring_oscilator`?

you can use it for true number generation. It is used a intial clocl source.
In application where clock is not important RP can function using the osicaltor for clock.
it oscilates so swithces between 1 and 0.
