# Compiler-Design-Projects
Compiler Design project implementing core compiler phases including lexical analysis, syntax analysis, semantic analysis, intermediate code generation, code optimization, and target code generation. Built to demonstrate compiler construction concepts and language processing techniques.
# Compiler Design Lab Experiments

This repository contains the implementation of the first six Compiler Design laboratory experiments using **LEX (FLEX)** and **YACC (BISON)**. These programs demonstrate the basic phases of compiler construction, including lexical analysis, syntax analysis, parsing, and expression evaluation.

## Technologies Used
- C Programming
- FLEX (LEX)
- BISON (YACC)
- GCC Compiler
- Linux / Ubuntu

## Experiments

### Experiment 1: Lexical Analyzer with Symbol Table
**Objective:**
Develop a lexical analyzer using FLEX to recognize identifiers, constants, comments, and operators in a C program while creating a symbol table for identifiers.

**Files**
- `symtab.l`

**Concepts Covered**
- Token recognition
- Symbol table generation
- Regular expressions

---

### Experiment 2: Lexical Analyzer using LEX
**Objective:**
Implement a lexical analyzer to identify keywords, identifiers, constants, operators, delimiters, header files, and preprocessor directives.

**Files**
- `lexer.l`

**Concepts Covered**
- Tokenization
- Pattern matching
- FLEX implementation

---

### Experiment 3: Arithmetic Expression Validation
**Objective:**
Recognize valid arithmetic expressions containing `+`, `-`, `*`, and `/` using FLEX and BISON.

**Files**
- `art_expr.l`
- `art_expr.y`

**Concepts Covered**
- Parsing
- Grammar rules
- Syntax validation

---

### Experiment 4: Variable Name Validation
**Objective:**
Recognize valid variable names that begin with a letter followed by letters or digits using FLEX and BISON.

**Files**
- `valvar.l`
- `valvar.y`

**Concepts Covered**
- Identifier validation
- Grammar construction
- Parser implementation

---

### Experiment 5: Control Structure Syntax Validation
**Objective:**
Validate the syntax of C language control structures such as `if`, `if-else`, `for`, `while`, and `switch-case` using FLEX and BISON.

**Files**
- `control.l`
- `control.y`

**Concepts Covered**
- Control statement parsing
- Grammar rules
- Syntax analysis

---

### Experiment 6: Calculator using LEX and YACC
**Objective:**
Implement a calculator capable of evaluating arithmetic expressions using FLEX and BISON.

**Files**
- `cal.l`
- `cal.y`

**Concepts Covered**
- Expression evaluation
- Operator precedence
- Arithmetic parsing

---

## How to Compile

### FLEX Only
```bash
flex filename.l
gcc lex.yy.c -o output -lfl
./output input.c
```

### FLEX + BISON
```bash
flex filename.l
bison -d filename.y
gcc lex.yy.c filename.tab.c -o output -lfl
./output
```

## Learning Outcomes
- Understand lexical analysis using FLEX.
- Learn syntax analysis using BISON.
- Build parsers using context-free grammars.
- Validate programming language syntax.
- Evaluate arithmetic expressions using parser rules.
- Gain practical knowledge of compiler design concepts.

## Author
** B SAKTHI PRIYAN **

## License
This repository is created for educational and academic purposes.
