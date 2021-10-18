# SIC-XE-Assembler
A simple implementation of SIC/XE assembler, written in python.

# Overview 
Simplified Instructional Computer (SIC) is a hypothetical computer that includes the
hardware features most often found on real machines. 

There are two versions of SIC,
1. SIC standard Model
2. SIC/XE (extra equipment or expensive)

In this repository, I implement the assembler of the latter.

SIC-XE instruction format : 

| 指令格式 |  | | | 長度 |
| ---|---|---|---|---|
| Type1 | Opcode : 8bits | | | 8bits |
| Type2 | Opcode : 8bits | Register1 : 4bits | Register2 : 4bits | 16bits |
| Type3 | Opcode : 6bits | n	i	x	b	p	e : 6bits | displacement : 12bits | 24bits |
| Type4 | Opcode : 6bits | n	i	x	b	p	e : 6bits | address : 20bits | 32bits |

demo picture : 

<pre>
                    input                                                       output(result)
</pre>

![image](https://user-images.githubusercontent.com/71260071/137664721-900a8745-34fd-46a0-8815-721a8c6e10c7.png)

# Requirements 
packages:
- numpy

# Usage 
1.Open git bash. 

2.Change the diretory where you want to do download this repository.
```
> cd (your directory)
```
3.Clone this repository. 
```
> git clone https://github.com/wei-0321/SIC-XE-Assembler.git
```
4.Change the diretory to this repository.
```
> cd SIC-XE-Assembler
```
5.Execute the program.
```
> python SICXE.py
```


# Project Structure
```
(Path)                                	 (Description)
SIC-XE-Assembler                         main folder     
│  │
│  ├ SICXE.py                            main program 
│  │
│  ├ input                               input directory
│  │  │
│  │  ├ example.txt                      the file you want to process
│  │
│  ├ output                              output directory
│  │  │
│  │  ├ example_result.txt               output result
│  │
