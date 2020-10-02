# silver-goggles
Hour Glass Kit firmware

This is a C program written for driving the 57 led hourglass kits available on sites like Banggood, ICStation, Ebay etc. It was compiled using the SDCC compiler for the STC15W201S mcu that comes with the kit. The mcu has 1K of program memory, 256 bytes of ram, and 4K of eeprom. The only hardware required to program the STC mcu is a USB to TTL serial converter like the CH340. STC-ISP is the free utility used to download the prgram and data to the STC. The new firmware allows you to display your own patterns. It cycles through each page. The pushbutton is used to adjust the speed it cycles. I have written a P5 JS program that can create the data for the display in the Intel hex format. The Javascript program can generate an Intel hex file that can be read by the STC-ISP software. The data is stored in the mcu eeprom. Each page or screen of data is stored in 12 bytes. The first 2 data bytes of the hex file are the number of pages.

Link to the P5 JS LED Editor:
https://editor.p5js.org/Rick100/full/TwRcbPRmD

