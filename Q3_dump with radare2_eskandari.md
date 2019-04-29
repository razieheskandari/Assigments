# Question:

Write a hello-world C program and explain how we can dump its binary code with radare2.

# Answer:

Write a hello world c program. 

![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(1).JPG)
 
 
The return value of main function are missed!!, but it is not imortant, since gcc will add it. =
Compile the program
 

![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(2).JPG)
 
Execute radar 2 from the reverse engineering tools in Kali.
Radare2 is an open source set of tools for reverse-engineering and analysis of binary files (among other things, for example debugging).
let's disassemble the hello program by running the following command:
 
![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(3).JPG)
 
At this point, analyze the whole code: aa (Analyze All)
Analyze all with aaa command then seek to main function
 
![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(4).JPG)
 
 The memory address changed to 0x00001135 (start of main function)

Now, we show the execution of the program step by step. let's see the main function: 
pdf @ sym.main (Print Disassemble Function)

![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(5).JPG)
  
As you see, it shows the hexadecimal code and the assembly code.
 
![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(6).JPG)
 
  
![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(7).JPG)
 

![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(8).JPG)
 

![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(9).JPG)
 

![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(10).JPG)

![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(11).JPG)

![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(12).JPG)

![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(13).jpg)

![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(14).JPG)

![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(15).JPG)

![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(16).JPG)

![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(17).JPG)

![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(18).JPG) 
  
![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(19).JPG) 

![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(20).JPG) 

![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(21).JPG) 

![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(22).JPG) 

![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(23).JPG) 

 
 

 
 
 
 
 
 


