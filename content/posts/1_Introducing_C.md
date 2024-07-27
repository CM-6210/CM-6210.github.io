+++
title = '1_Introducing_C'
date = 2024-07-28T01:24:26+09:00
draft = false
tags = ["programming","c","study"]
categories = ["Programming","C","Study"]
+++
# 1-1 History Of C
## Origins
UNIX was written in assembly.  
- -> painful  
- -> Thompson designed "B"  
- -> Ritchie joined, and rewrote a portion of UNIX in B  
- => It became C --> Benfit: portability  

## Standardization
1970s: C evolved & evolved  
80s: C hd expanded(UNIX), C compilers could run under different OS  
K&R was fuzzy about some language features.  
- U.S. Standard for C began(1983)  
- (American National Standards Institute,ANSI의 후원)  
- -> C89, C90  
and NEW standard C99  
## C-based Langs
C++,JAVA,C# 등 -> 이런 거 유명하고 많이 쓰이는데 C 왜 배움?  
- -> greater insight into C-based langs  
- -> older C programs that we may need to read,maintain  
- -> 아직 널리 쓰임  

# 1-2 C의 장단점
## C's underlying philosophy
1. **low-level**: closely to a computer's built-in instructures.
2. **Small**: number of features small
3. **permissive**: 내가 하는 것에 간섭 ↓

## 장단점
### 장점
- portability
- power
- flexibility
- standard lib
- Intergration with UNIX
### 단점
- 에러가 나기 쉬움
- 이해하기 어려울지도
- hard to modify

## Effective use of C
-> Taking advantages/avoid weaknesses
- Learn how to avoid C pitfalls
- Use software tools to make programs mroe reliable
- Take advantage of existing code lib
- Adopt a sensible set of coding conventions
- Avoid 'tricks' and overly complex code
- Stick to the standard