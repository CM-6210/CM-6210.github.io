+++
title = '2_C_Fundamentals'
date = 2024-07-28T19:27:30+09:00
draft = true
+++
# 2-1 Writing a Simple Program
### Printing a Pun
Here's the pun: To C, or not to C: that is the question.
pun.c 라고 이름을 지을 아래 프로그램은, 실행될 때 위 메시지를 보여준다.
```C
#include <stdio.h>

int main(void)
{
	printf("To C, or not to C: taht is the question. \n");
	return 0;
}
```
섹션 2-2에서 자세한 설명. 지금은 간단하게만
"#include <stdio.h>". 이것은 C's standard I/O(INPUT/OUTPUT)을 include 하기 위해 필요하다.
프로그램의 executable code는 main 안에 있다. main은 "main"프로그램을 나타낸다.
printf는 nicely formatted output을 produce하는 standard I/O lib의 function이다. "\n"은 printf에게 advance to the next line after printing the message하라고 말한다.
"return 0;"은 프로그램이 끝났을 때 Operating System에게 0의 값을 return하라는 것을 나타낸다.

# Compiling and Linking
pun.c를 run하려면
1. create a file named pun.c containing the program
2. Convert the program to a form that the machine can execute.
### For C programs
usually involves three steps:
#### Processing
The program is first given to a preprocessor, which obeys ommands that begin with #(known as directives). A preprocessor is like an editor. It can add things to the program and make modifications.
#### Compiling
The modified program now goes to a compiler, which translates it into machine instructions(Object Code). The program isn't quite ready to run yet.
#### Linking
A linker combines the object code with any additional code needed to yield a complete executable program. This additional code includes lib functions (ex) printf) that used in the program.

다행이도, this process is often automated. 사실 preprocessor는 compiler와 통합되어 있는 경우가 많음. 아마 그래서 알아차리지 못할수도. compile하고 link하는데 쓰이는 commands는 컴파일러와 OS에 따라 다르다. 간단하게 gcc를 소개하자면

------------------------------
### GCC COMPILER
- one of the most popular C compilers
- supplied with Linux, but now available for many other platforms
- EX) to compile pun.c -> gcc -o pun pun.c
----------------------------------
