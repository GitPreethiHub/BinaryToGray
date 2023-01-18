# BinaryToGray

## Aim:

    To impement 5-bit Binary to Gray code converter using verilog and validating their functionality.

## Theory:

    The Binary to Gray code converter is a logical circuit that is used to
       convert the binary code into its equivalent Gray code.
    The circuit of Binary to Gray code converter is shown in the following figure

![images](https://static.javatpoint.com/tutorial/digital-electronics/images/binary-to-gray-code-cconversion.png)
    
    In the Gray code, the MSB will always be the same as the 1'st bit of the given binary number.
    In order to perform the 2nd bit of the gray code, we perform the exclusive-or (XOR) of the
      1'st and 2nd bit of the binary number. It means that if both the bits are different,
      the result will be one else the result will be 0.
    The process remains the same for the 3rd 4th and 5th bit of the Gray code.

## Procedure:

    Compile and run the verilog program in the quartus software.
    Realize the RTL logic for the same.
    Create a new university program vwf and import nodes using node finder.
    Run functional simulation to obtain the timing diagram.

## Program:
    
     /*
     Program for 5-bit Binary to Gray code converter in quartus using Verilog programming.
     Developed by: Preethi M
     RegisterNumber:  22000091
      */
       module BINtoGRAY(a,b,c,d,e,y1,y2,y3,y4,y5);
      input a,b,c,d,e;
      output y1,y2,y3,y4,y5;
      assign y1=a;
      xor(y2,a,b);
      xor(y3,b,c);
      xor(y4,c,d);
      xor(y5,d,e);
      endmodule
      
## Truth table for 5-bit Binary to Gray code converter:

![BINtoGRAYtruth](/images/BINtoGRAYtruth.png)

## RTL logic for 5-bit Binary To Gray code converter:

![BINtoGRAYrtl](/images/BINtoGRAYrtl.png)

## Timing diagram for 5-bit Binary To Gray code converter:

![BINtoGRAYsim](/images/BINtoGRAYsim.png)

## Result:

    Thus the 5-bit binary to gray code converter is successfully implemented using verilog and it's
    functionality is validated.
