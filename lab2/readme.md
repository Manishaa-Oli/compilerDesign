# Lab 2: Lexical Analyzer for Token recognition using flex
## Title: Lexical Analyzer for token recognition using Flex
## Objective:
 To design and implement a lexical analyzer using Flex that reads a C-like program and identifies tokens such  as:

• Keywords 

• Identifiers 

• Operators 

• Numbers 

• Special Symbols 

• Separators

## Software Requirements
### Flex : Lexical Analyzer Generator
### GCC : C compiler to compile generated code
### OS : Windows (MinGW)

## Theory

A lexical analyzer reads the source code character by character and groups characters into 
meaningful sequences called tokens. 
Tokens in C include: 

•       Keywords: if, else, int, float, return, ... 

•       Identifiers: variable or function names

•       Operators: +, -, *, /, = 

•       Numbers: 1, 2, 3, etc. 

•       Special Symbols: ;, (, ), {, }, etc.

## Compilation order

1. Save the program file as .l

2. Generate C source file `<filename>.l` which generates lex.yy.c
3. comfile the program as` gcc lex.yy.c -o <filename>`
4. Run the program `./<filename>`

## Sample input

`int a=5;`

 `printf("enter the number");`

## Output

`Keyword: int`

`Identifier: a`

`Operator: =`

`Number: 5`

`Separator: ;`

`Identifier: printf`

`Separator: (`

`Unknown symbol: "`

`Identifier: enter`

`Identifier: the`

`Identifier: number`

`Unknown symbol: "`

`Separator: )`

`Separator: ;`

## Discussion and Conclusion

The lexical analyzer was successfully designed and implemented to scan the input source code and convert it into meaningful tokens such as keywords, identifiers, operators, and constants. It effectively removes unnecessary characters like whitespaces and comments, and identifies the lexical structure of the program. This experiment helped in understanding the first phase of compiler design and the role of token generation in simplifying the parsing process for syntax analysis.