# EXPERIMENT--01-ALP-FOR-8086
### Name : ANUBHARATHI SS
### Roll no : 212223040017
### Date of experiment : 29.08.2025





## Aim: To Write and execute ALP on fundamental arithmetic and logical operations
## Components required: 8086  emulator 
## Theory 
Running The Emulator (emu8086) Intro 8086 Microprocessor Emulator, also known as EMU8086, is an emulator of the program 8086 microprocessor. It is developed with a built-in 8086 assembler. This application is able to run programs on both PC desktops and laptops. This tool is primarily designed to copy or emulate hardware. These include the memory of a program, CPU, RAM, input and output devices, and even the display screen. There are instructions to follow when using this emulator. It can be executed into one of the two ways: backward or forward. There are also examples of assembly source code included. With this, it allows the programming of assembly language, reverse engineering, hardware architecture, and creating miniature operating system (OS). The user interface of 8086 Microprocessor Emulator is simple and easy to manage. There are five major buttons with icons and titles included. These are “Load”, “Reload”, “Step Back”, “Single Step”, and “Run”. Above those buttons is the menu that includes “File”, “View”, “Virtual Devices”, “Virtual Drive”, and “Help”. Below the buttons is a series of choices that are usually in numbers and codes. At the leftmost part is an area called “Registers” with an indication of either “H” or “L”. The other side is divided into two, which enables users to manually reset, debug, flag, etc. What is 8086 emulator emu8086 is an emulator of Intel 8086 (AMD compatible) microprocessor with integrated 8086 assembler and tutorials for beginners. Emulator runs programs like the real microprocessor in step-by-step mode. it shows registers, memory, stack, variables and flags.


 ## Running the Emulator :
1.	Download and install emu8086 (www.emu8086.com) It is usually installed in C:\EMU8086 subfolder in the “Windows” directory
2.	  Run  emu8086 icon (on the desktop or in the c:\EMU8086 folder of window) It has green color 
 
 
3.		write the code for the appropriate program for ADDITION,SUBTRACTION, MULTIPLICATION,  DIVISION operations 

4.	 Compile the program and check for the errors 
5.	Run (once there is no syntax error) 

6.	Click OK to see/view the output of your program on the Emulator screen. 


7.	After running the program, another menu screen will be displayed, where you have the option to “View” symbol table,
8.	 


![image](https://user-images.githubusercontent.com/36288975/189273263-d65baae9-4b8f-4723-afb3-c0ffa4052b04.png)











9.	Click on emulate to start emulation 








![image](https://user-images.githubusercontent.com/36288975/189273273-9bb36ec1-e2e8-4892-8d35-37707332bfdc.png)








10.	If no errors are found click on run the program and check the status of various flags in the flags tab as shown below 






![image](https://user-images.githubusercontent.com/36288975/189273277-113a2a33-4a40-4ff8-95a5-ecd3a1f504fe.png)







## Programs for arithmetic  operations

## Addition  of 8 bit ALP 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
ADD AX,BX
JNC Loop
INC CL
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT
```


## Output  
<img width="1920" height="1080" alt="Screenshot (220)" src="https://github.com/user-attachments/assets/2fbf049f-4b93-4612-996c-8d101acc82f6" />

 
## Subtraction   of 8 bit numbers  ALP 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
SUB AX,BX
JNC Loop
INC CL  
NOT AX
INC AX
Loop:
MOV [3005H],AX
MOV [3007H],CL
HLT
```
## Output  
<img width="1920" height="1080" alt="Screenshot (221)" src="https://github.com/user-attachments/assets/b394343c-bf5b-4301-885d-2e10e671fbc3" />


## Multiplication alp 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
MUL BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```
## Output  
<img width="1920" height="1080" alt="Screenshot (222)" src="https://github.com/user-attachments/assets/dcc02622-71d9-4c71-bc75-d8df1c8e53dd" />


## Division alp 
```
MOV CL,00
MOV AX,[3001H]
MOV BX,[3003H]
DIV BX
MOV [3005H],AX
MOV [3007H],DX
HLT
```

## Output  
<img width="1920" height="1080" alt="Screenshot (223)" src="https://github.com/user-attachments/assets/ee68a208-7d78-4a92-8664-5268c323281f" />

## Logic operation
## AND 
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
MOV [3005H],AX
HLT

```
## OUTPUT
<img width="1920" height="1080" alt="Screenshot (224)" src="https://github.com/user-attachments/assets/127ff750-998d-4d3b-b43f-92dca8f44f4b" />

## NAND 
```
MOV AX,[3001H]
MOV BX,[3003H]
AND AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## OUTPUT
<img width="1920" height="1080" alt="Screenshot (225)" src="https://github.com/user-attachments/assets/7dd3c789-bea1-43f0-8b17-158c00b04a6d" />

## OR 
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
MOV [3005H],AX
HLT

```
## OUTPUT
<img width="1920" height="1080" alt="Screenshot (214)" src="https://github.com/user-attachments/assets/36ce5023-4c03-441a-b8f9-74b892c173bf" />

## NOR
```
MOV AX,[3001H]
MOV BX,[3003H]
OR AX,BX
NOT AX
MOV [3005H],AX
HLT

```
## OUTPUT
<img width="1920" height="1080" alt="Screenshot (226)" src="https://github.com/user-attachments/assets/76c3dcbc-32b7-4b40-8a92-7e4a2ffb2b30" />

## NOT
```
MOV AX,[3001H]
NOT AX
MOV [3003H],AX
HLT

```
## OUTPUT
<img width="1920" height="1080" alt="Screenshot (217)" src="https://github.com/user-attachments/assets/99b24c7f-e245-4c90-95f1-32ed260a894e" />

## XOR
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
MOV [3005H],AX
HLT

```
## OUTPUT
<img width="1920" height="1080" alt="Screenshot (227)" src="https://github.com/user-attachments/assets/1bbc6b73-fe8f-4c08-a3ae-3de33ab6441e" />

## XNOR
```
MOV AX,[3001H]
MOV BX,[3003H]
XOR AX,BX
NOT AX
MOV [3005H],AX
HLT
```
## OUTPUT
<img width="1920" height="1080" alt="Screenshot (218)" src="https://github.com/user-attachments/assets/b8280b6d-3176-4b1a-95bb-348305322af4" />



## Result :
Thus the program was executed successfully.
 








