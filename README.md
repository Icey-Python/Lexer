# Lexical Analyzer Assignment

This repository contains solutions to a set of lexical analyzer assignments using Flex (Fast Lexical Analyzer Generator).

## Project Structure

The project is organized into three separate questions/solutions:

- **Q1**: Word Count Analyzer
- **Q2**: Text Capitalizer
- **Q3**: Verb Recognizer

## Solutions

### Q1:(1.a) Word Count Analyzer

A lexical analyzer that counts the total number of words in a text file and calculates their combined size in characters.

**Files:**
- `verb_recognizer.1`: The Flex source file
- `lex.yy.c`: The C code generated by Flex
- `verb_recognizer`: The compiled executable
- `input.txt`: Sample input text for testing

**Usage:**
```bash
cd Q1
flex word_counter.1
gcc lex.yy.c -o word_counter -lfl
./verb_recognizer < input.txt
```

### Q2:(1.b) Text Capitalizer

A lexical analyzer that capitalizes text from the input.

**Files:**
- `capitalize.1`: The Flex source file (binary)
- `lex.yy.c`: The C code generated by Flex
- `input.txt`: Sample input text for testing

**Usage:**
```bash
cd Q2
flex capitalize.1
gcc lex.yy.c -o capitalize -lfl
./capitalize < input.txt
```

### Q3:(2) Verb Recognizer

A lexical analyzer that identifies and extracts common English verbs from text.

**Files:**
- `verb_recognizer.1`: The Flex source file
- `lex.yy.c`: The C code generated by Flex
- `input.txt`: Sample input text containing verbs for testing

**Usage:**
```bash
cd Q3
flex verb_recognizer.1
gcc lex.yy.c -o verb_recognizer -lfl
./verb_recognizer < input.txt
```

## How to Compile Flex Programs

Each solution can be compiled using the following general steps:

1. Generate C code from the Flex source file:
   ```bash
   flex filename.l
   ```

2. Compile the generated C code:
   ```bash
   gcc lex.yy.c -o output_name -lfl
   ```

3. Run the program with input:
   ```bash
   ./output_name < input.txt
   ```

## Requirements

- Flex (Fast Lexical Analyzer Generator)
- GCC (GNU Compiler Collection)

## License

This project is provided for educational purposes. 