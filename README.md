# Z80 Modular Computer     _Writeup still in progress_
A modular Z80-based computer using through-hole perfboard.
## Background
This project started back during high school due to an interest in computer systems and to gain a better understanding of how CPU's interact with other system components. Due to being younger, proper engineering methods were not followed for this and was more of a fun spare time project.
The goal was to eventually have a working analog video interface and a basic UI. The video card was started, but due to having minimal understanding of Machine Code and Assembly at the time, the project ended up sitting for a while.
This is just a summary of the build process and overall design to add to a portfolio of projects and also to get used to using Markdown and GitHub as a project portfolio. This will be updated or continued on with another repo if this project is completed in the future.

## Build
The computer was built with a modular design in mind where the CPU, memory, ROM and control logic were on the main board and IO, video and more would be modular add-ons connected by standard through-hole pin headers. All boards were made by using basic perfboard and soldering single-core wires underneath as traces.\
_Entire project:_
![Image1](/images/image6.jpg "Entire Z80 Computer")\
_Bottom Side:_
![Image2](/images/image4.jpg "Bottom side")
### The Zilog Z80 CPU
The Zilog z80 cpu was chosen due to it's simplicity compared to modern systems and easy to work with through-hole footprint.
### Electrical Connections
Each routing was creating by hand soldering lengths of single-core wire between joints. Being single-core, this allowed the 'traces' to stay rigid when bent and made it easier to organise, even though it was an overall messy (but fun) way of doing things.\
Boards were connected by using 2.54mm-spaced throughhole headers. While not extremely stable and required careful handling when connecting and disconnecting modules, this made it very straight forward to put together initially.
## Programming
The board was programmed using a Xgecu TL866ii usb chip programmer (which involved physically removing the ROM IC from its socket and clamping into the programmer). The EEPROM chip used was a 64Kbit Atmel at28c64b. A 27C64 UV erasable EPROM was also used at one point for the fun of it.\
A basic LED output binary counter program was written in assembly at the time, but required manual clock pulsing to be slow enough to see.\
## Revisiting (2026)

