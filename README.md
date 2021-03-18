UART From RTL to GDS-II
-----------------------
The Design's Feautures:
| Feauture       | value   |
| -----------    | ------- |
| Frequency      | 150 MHZ |
| Baud Rate      | 9600    |
| Sampling Rate  | 16x     |
|  Divisor Value | 977     |
  
**_Description_** 
  --------------
*A universal asynchronous receiver-transmitter(UART) is a computer hardware device for asynchronous serial communication in which the data format and transmission speeds are configurable.
*Configurable means that it can be adjusted to several standard rates for transmitting and recieving, which is slow relative to the original clock.
*This is via hardware design and implementation  which is slow relative to the original clock.
*The code here is specific for baud rate 9600 only.
*In the top design you'll find instances from the transmitter and the reciever.
*In both transmitter and reciever we instansiate the baud-rate generator that generates clock 16x times faster than the original clock, to sample the recieved bits and transmit the data relative to this clock.
*16x faster than the baud rate means that every recieved and transmitted bit will contain 16 cycles of 

