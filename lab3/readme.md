## Lab 3: Token Counters for Identifiers,Keywords and Operators Using Flex

### Objective:
-To develop lexical analyzer using flex that scans input code and:
 
 - Identifies tokens like keywords,identifiers,numbers,operators and comments.

 -Counts how many of each token type appears.

 ### Software Requirements:

 -Flex

 -GCC

 -OS

 ### Theory
 A Token Counter is a lexical analysis tool used to identify and count different types of tokens in a source program. Tokens are the smallest meaningful units of a programming language, such as keywords, identifiers, and operators. In compiler design, lexical analysis is the first phase that scans the input program and classifies these tokens.
 Flex (Fast Lexical Analyzer Generator) is a tool used to generate lexical analyzers automatically using regular expressions

 ### Compilation Order
 - Save the file as token_counter.l

 - Generate the lexical analyzer using Flex:
   `win_flex token_counter.l`

 - Compile the generated C source file:
   `gcc lex.yy.c -o token_counter`
 
 - execute the program: `./token_counter`

 - enter the source code as input.

 - The program scans the source code,identifies    tokens , and counts keywords,identifiers and operators.
 - Press Ctrl + Z and then Enter to terminate the input 

 - Display the total count of each token category.

 ## Conclusion
 The Token Counter program using Flex successfully identifies and counts different types of tokens such as keywords, identifiers, and operators from a given source program. It demonstrates the working of lexical analysis, which is the first phase of compiler design. By using regular expressions in Flex, the program efficiently scans the input code and categorizes each token. This experiment helps in understanding how compilers break source code into meaningful units and provides a basic foundation for building lexical analyzers.