# Intermediate-Code-Genaration
A minimal C compiler implementation in flex and bison. The input will be a C source program in .c extension. On the other hand, there will be two output file.
One file, _log.txt_, that will contain line count, error count and any lexical, syntax or semantic errors. Another file, _code.asm_ will contain the generated assembly code
before performing optimization. The last file _optimizedCode.asm_ will contain the assembly code after optimization. 

Our chosen subset of C language has following characteristics.
* There can be multiple functions. No two function will have the same name. A function need to be defined or declared before it is called. Also a function and a global variable cannot have the same symbol.
* There will be no preprocessing directives like include or define.
* Variables can be declared at suitable places inside a function. Variables can also be declared in global scope.
* All the operators used in previous assignment are included. Precedence and associativity rules are as per standard. Although we will ignore consecutive logical operators or consecutive relational operators like ‘a && b && c’ ‘a < b < c’.
* No break statement and switch-case.

## To Run

run _script.sh_.  
open _code.asm_ in emu8086.
