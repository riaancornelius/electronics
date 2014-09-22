### Product Description

The Bare Bones Board (BBB) is an Arduino-compatible board (Freeduino) that implements the functionality of the Arduino Duemilanove/Diecimila, on a smaller printed circuit board, by removing the USB communications chip to another board.

The Bare Bones Board is completely compatible with the Arduino project software and IDE. Currently the Bare Bones Board is listed on the Arduino site as “Recommended Third-Party Hardware”. It has also gained a devoted following among Arduino users, as a convenient, effective, and low-cost hardware solution.

The BBB is programmed with the USB-BUB Board or equivalent FTDI cable or adapter board. This saves the cost of repeatedly paying for the communications chip, in future projects. It also allows the BBB to be 1/3 smaller in both dimensions than the Arduino® Duemilanove board.

### Specifications

#### Bare Bones Board (BBB) features

Despite the Bare-Bones name, the BBB is a full featured Arduino-compatible that includes the vast majority of the functionality of the Arduino Duemilanove.

* Standard with the latest 328 chip for more memory and faster uploads.
* Programmed by a USB-BUB Board or FTDI cable.
Designed with all through-hole parts for easy assembly by beginners.
* The BBB can be built in many configurations for custom projects.
* Designed with male header pins on bottom to insert directly into solderless breadboards, saving a lots of wiring and fuss.
* Analog inputs have adjacent +5V and Ground buses to make interfacing sensors easy by using a three pin female header or servo cable.
* Flexible power options (USB/External) and an onboard voltage regulator that can be used with either TO92 or TO220 (7805 or LM2940 ) voltage regulators.
* Convenient pins to power, (or draw power from) breadboard power buses, a shunt allows easy switching between options.
* Optimizes breadboard space by hanging over the edge of the breadboard. This allows an LED and resistor to be conveniently wired to one BBB pin for example (see photo).
Includes an inductor for high frequency noise filtering on the analog system reference input.
* 2.35″(59.7mm) * 1.60″(40.6mm)

Arduino is programmed in the “C” programming language, with an integrated development environment (IDE) engineered for beginning programmers. The language includes support for desirable microcontroller features such as 32 bit and floating point math and many standard C libraries. Projects that outgrow the Bare-Bones Board’s capabilities can easily be ported to the Wiring v.1 Board, which is based on the Atmega128 chip, or the Wiring S or Sanguino, which is based on the Atmega644.

#### Atmega328 features, upon which the BBB is based

* 32k flash program storage
* 2k RAM for program memory
* 6 PWM outputs
* 6 A/D inputs
* UART and SPI interfaces
* Hardware interrupts
* 20 general purpose I/O pins (shared with PWM and Analog pins)
* 16 MHz RISC microcontroller
* Open-source hardware, IDE, bootloader
* Easy upgrade to more powerful hardware (Wiring)

#### History / Design

The BBB was the first Freeduino (Arduino not designed by "the Arduino Team"), around 2007. At the time it was called the "Bare Bones Arduino" because the Arduino Team hadn't started asking people not to use not to use the term "Arduino" in their designs (hence all the "duino" suffixes later). And way before the Arduino team applied for a trademark and got rejected, and hired more lawyers and finally got their trademark; but I digress.

In any case I wanted an Arduino that would sit on a breadboard and didn't have the now somewhat infamous .060 gap between the front pins that hackers hate. Also I didn't want the FTDI chip on the board as it tends to make the Arduino boards larger, more expensive and use more power. I also wanted a board students could build themselves and hackers could easily mod or build into their own designs. So I designed a board to work with the FTDI cables that had just appeared on the market, and we used them in classes for a couple of semesters before I ever spun a board for general sale.

The analog-block headers had auxiliary power and ground pins to make interfacing analog sensors easy. The original analog-block had a .100" gap to polarize the header so people wouldn't get plugs in backwards. Later Brian Riley, of Wulfden.org, convinced me that the gap should be eliminated, so that a standard servo cable to could be used to interface sensors (and also servo motors - although this has some significant power limitations, so is not ideal for servos).

Over the years various tweaks have been added on such as holes that will accommodate either a TO-92 or TO-220 regulator and changing the routing of the USB power through the regulator. There was a point to that, since the current regulator tended to limit the amount of power the board asked from a USB port - with a short circuit, but the regulator would skim off a few millivolts and the board would always ending up running at 4.85 volts instead of 5 volts.

Story and documentation to be continued ...

### References

* [BBB RevE Assembly and Instructions](./BBB_RevE_Instructions03.pdf)