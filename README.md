# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: Pavan kishore.M
RegisterNumber:  2122212230076


Half adder program:

module fulladd (a,b,sum,carry);
input a,b;
output sum,carry;
assign sum = (a^b);
assign carry = (a&b);
endmodule

Full adder program:

module fulladd (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = (a^b^c);
assign carry = ((a&b)|(a^b)&c);
endmodule

### output:
### RTL
Half adder:
![op1](https://user-images.githubusercontent.com/94154941/164907922-7e5d22e6-83cb-4695-8dcf-6f020ee3b550.png)
Full adder:
![op2](https://user-images.githubusercontent.com/94154941/164908932-99e1ab04-3c5e-410c-908f-ede17385a868.png)



### TIMING DIAGRAM
Half adder:
![opp1](https://user-images.githubusercontent.com/94154941/164908940-689b707e-b077-4321-a851-8ed8f4f42a29.png)

Full adder:
![opp2](https://user-images.githubusercontent.com/94154941/164908941-1a572e94-7d35-444c-838f-324276e03a6a.png)


### TRUTH TABLE 
Half adder:
![oppp1](https://user-images.githubusercontent.com/94154941/164908952-7360c322-b3ee-4237-b50a-4cab81e00e2a.png)
Full adder:
![oppp2](https://user-images.githubusercontent.com/94154941/164908965-3e9bccd4-2514-4cc2-aa54-684a43e230d8.png)


### Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.
