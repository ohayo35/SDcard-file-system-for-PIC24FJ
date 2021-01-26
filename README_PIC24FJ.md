This C based SDcard file system for PIC24FJ 16 bits PICs is based on the FatFs file system open source project : http://elm-chan.org/fsw/ff/00index_e.html

It has been tested in the following environment :

Software : 
MPLAB X v5.45 IDE, 
XC16 v1.61 C compiler,
MCC plugin for MPLAB X v4.0.2 with Core v5.0.2,
MCC FatFs library v1.1.0

Hardware :
EXPLORER1632 (DM240001-3),
PIC24FJ128GA204  ( PIM MA240037 ),
microSD card click (ref 924 from Mikroelektronika) on interface B socket,
=> tested on 2GB / 8GB or 64GB microSD cards (must be formated for FAT32),
NB : to format uSD cards >= 32GB use open source application "FAT32 format",
This project uses SPI2 as SPI1 is already used by the EEPROM on the EXPLORER1632.
 
The project attached demonstrate how to create a text file and write a couple of sentences in it. The microSD card can then be easily read on a PC as it uses a standard file system (FAT32) It uses MCC (MPLAB Code configurator) and makes it simple to port to any other 16 bits PIC24FJ device. SPI communications is setup for 400kHz
