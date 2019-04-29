# Question:

Write a hello-world C program and explain how we can dump its binary code with radare2.

# Answer:

Write a hello world c program. 

![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(1).JPG)
 
 
The return value of main function are missed!!, but it is not imortant, since gcc will add it. =
Compile the program
 

![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(2).jpg)
 
Execute radar 2 from the reverse engineering tools in Kali.
Radare2 is an open source set of tools for reverse-engineering and analysis of binary files (among other things, for example debugging).
let's disassemble the hello program by running the following command:
 
![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(3).jpg)
 
At this point, analyze the whole code: aa (Analyze All)
Analyze all with aaa command then seek to main function
 
![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(4).jpg)
 
 The memory address changed to 0x00001135 (start of main function)

Now, we show the execution of the program step by step. let's see the main function: 
pdf @ sym.main (Print Disassemble Function)

![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(5).jpg)
  
As you see, it shows the hexadecimal code and the assembly code.
 
![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(6).jpg)
 
  
![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(7).jpg)
 

![alt text](https://github.com/razieheskandari/Screenshots/blob/master/Q3(8).jpg)
 

![alt text] (https://github.com/razieheskandari/Screenshots/blob/master/Q3(9).jpg)
 

![alt text] (https://github.com/razieheskandari/Screenshots/blob/master/Q3(10).jpg)

![alt text] (https://github.com/razieheskandari/Screenshots/blob/master/Q3(11).jpg)

![alt text] (https://github.com/razieheskandari/Screenshots/blob/master/Q3(12).jpg)

![alt text] (https://github.com/razieheskandari/Screenshots/blob/master/Q3(13).jpg)

![alt text] (https://github.com/razieheskandari/Screenshots/blob/master/Q3(14).jpg)

![alt text] (https://github.com/razieheskandari/Screenshots/blob/master/Q3(15).jpg)

![alt text] (https://github.com/razieheskandari/Screenshots/blob/master/Q3(16).jpg)

![alt text] (https://github.com/razieheskandari/Screenshots/blob/master/Q3(17).jpg)

![alt text] (https://github.com/razieheskandari/Screenshots/blob/master/Q3(18).jpg) 
  
![alt text] (https://github.com/razieheskandari/Screenshots/blob/master/Q3(19).jpg) 

![alt text] (https://github.com/razieheskandari/Screenshots/blob/master/Q3(20).jpg) 

![alt text] (https://github.com/razieheskandari/Screenshots/blob/master/Q3(21).jpg) 

![alt text] (https://github.com/razieheskandari/Screenshots/blob/master/Q3(22).jpg) 

![alt text] (https://github.com/razieheskandari/Screenshots/blob/master/Q3(23).jpg) 

 
 

 
 
 
 
 
 


