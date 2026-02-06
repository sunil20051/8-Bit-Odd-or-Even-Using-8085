# 8-Bit-Odd-or-Even-Using-8085

## Aim:
To write an 8085 microprocessor program to check whether a given 8-bit number is odd or even.

## Apparatus Required:
•	Laptop with an internet connection

## Algorithm:
1.	Load the number from a specified memory location into register A.
2.	Perform an AND operation with 01H to check the least significant bit (LSB).
3.	If the result is 0, the number is even; otherwise, it is odd.
4.	Store the result in a specific memory location (odd or even flag).


## Program:
```
LDA 4200H       
ANI 01H         
JZ EVEN 
JMP ODD
EVEN:
MVI A, 01H  
STA 4201H
HLT       
ODD: MVI A,02H
STA 4201H
HLT
```

## Output:
EVEN:
<img width="1898" height="915" alt="image" src="https://github.com/user-attachments/assets/6e5b52a2-0f97-4b01-bb32-27a2da9d8f81" />
ODD:
<img width="1917" height="917" alt="image" src="https://github.com/user-attachments/assets/846387cd-59da-48b7-aeeb-050dd3e4c5ce" />

Verification:

![WhatsApp Image 2026-02-06 at 9 25 44 AM](https://github.com/user-attachments/assets/070af508-df6c-4486-83e1-1e032192406c)



## Result:
The 8085 microprocessor successfully checks whether a given number is odd or even and stores the result in memory.

