![](../../workflows/gds/badge.svg) ![](../../workflows/docs/badge.svg)

# CNS Test Submission 2
## Sequential ALU

* Authors: Bryan Bonilla Garay, Devin Alvarez, Ishaan Singh, Yu Feng Zhou and N. Sertac Artan




* Description: A clock with three clock cycles that takes in two 5-bit numbers and performs a addition/subtraction operation. The result is output to a 7-segment display.
* [GitHub repository](https://github.com/NYIT-CNS/cns002-tt02-submission2)
* [Wokwi](https://wokwi.com/projects/349893893465047635) project
* Clock: 0 Hz
* External hardware: None  

### How it works
On the first Toggle cycle the first number (on inputs D4-D0) is saved onto a 5-bit register, the same happened in the second toggle but in a seperate 5-bit register. On the thrid Toggle cycle the operation code is read from D0 and the operation is perform, the result is stored in a 6-bit register.




### How to test
Using default settings, enter a binary number into pins D4-D0, where D0 is LSB, once the number is set on the pins, toggle, then input the second number. Toggle again, then input the operation, toggle once more to have the result saved in the chip. You can then use the Disp pin 7 to display either the LSD (0) or MSD (1).





### IO

| # | Input        | Output       |
|---|--------------|--------------|
| 0 | Clock |  segment a  |
| 1 | D0  |  segment b  |
| 2 | D1 |  segment c  |
| 3 | D2 |  segment d  |
| 4 | D3  |  segment e  |
| 5 |  D4  |  segment f  |
| 6 | Toggle   |  segment g  |
| 7 |  Display  |  segment dp  |
