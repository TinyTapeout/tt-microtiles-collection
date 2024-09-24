<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works

The objective of this work is to design a chip module which performs 1-bit error
detection and correction in the transmitted encoded data.
The proposed design includes three sections: a transmitter, built in self-test
block (for testing purposes), and a receiver.
The transmitter takes an 8-bit input and generates 4 redundant bits, creating a
12-bit encoded data stream for transmission.
The second block is used as built in self-test block(BIST). This block is used to
intentionally insert an error during transmission of encoded data to properly test
our design. If no error is inserted in the transmitted code word, 4 output pins
display the redundant bits. However, If 1-bit error is provided, these pins
display the error position.
The receiver block can correct any 1-bit error in the received 12-bit data and
displays the corrected data as provided at the input side.

## How to test
This design has 8-input data pins which will use to provide digital input bits, 8 output pins will use to check the output by connectings LED's. Four birectional pins will use as a input ports for BIST and remaining four bidirectional pins will use as output pins to detect the postion of the error.

## External hardware

Twelve LED's, LED Display, four bit counter, Eight bit counter and Twelve digital input switch
