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
/*
HALF ADDER

module exphalf(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b);
endmodule

FULL ADDER

module expfull(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = ((a^b)^c);
assign carry = ((a&b)|(b&c)|(c&a));
endmodule

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

###Developed by: HARI PRASATH S
###RegisterNumber: 212222240034

*/
Logic symbol & Truthtable
RTL realization

### RTL
HALF ADDER

![267689047-a7cc3d34-404f-43f5-9cbc-d9f5f5ba28e9](https://github.com/hariprasath5106/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/111515488/f7544eb0-ad08-429c-901e-3001484f9dc8)

FULL ADDER

![267689278-7667c24f-a414-4e2b-840e-2ce0335dfbae](https://github.com/hariprasath5106/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/111515488/ae7a6204-141c-4acb-940e-ec8a629ffad4)


### TIMING DIAGRAM
HALF ADDER
![267689451-61076839-9c19-4192-a86a-d7233a325961](https://github.com/hariprasath5106/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/111515488/69b19c9d-c756-4191-99a2-a74ff51eb977)

FULL ADDER

![267689613-e5f0bbf9-9197-4bbf-a392-1e1dcad2f804](https://github.com/hariprasath5106/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/111515488/8a830c8d-1b5c-476a-af04-809b624b9dd1)


### TRUTH TABLE 
HALF ADDER

![267688455-b8abff6e-d197-4edd-9219-a69d9cb76aa8](https://github.com/hariprasath5106/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/111515488/8d1211e9-eb1c-4266-97f1-7d10dbf9107b)

FULL ADDER

![267688520-7278c4df-a0ac-43c2-b0e0-75a0dffe843a](https://github.com/hariprasath5106/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/111515488/372bc6b4-cafb-4003-abf8-ece9be1c48ee)
 
### Result:
Thus the different digital IC's are studied and the truth table for different logic gates are verified.
