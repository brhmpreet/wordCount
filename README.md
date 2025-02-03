# ccwc

ccwc counts various statistics of a text file, such as the number of lines, words, characters, and bytes. It takes command-line arguments to specify the operation and the file to be analyzed.

It supports four different options:

1. `-l`: Count the number of lines in the input file.
2. `-w`: Count the number of words in the input file.
3. `-c`: Count the number of bytes in the input file.
4. `-m`: Count the number of characters in the input file (same as `-c` if the current locale does not support multibyte characters).

It also handles input from standard input (stdin) if no fileName is specified.


## How to Run

To compile and run this C++ program, follow these steps:

1. Make sure you have a C++ compiler installed on your system (e.g., g++ for Unix-like systems or Visual C++ for Windows).

2. Save the code to a file with a `.cpp` extension, such as `ccwc.cpp`.

3. Open a terminal or command prompt and navigate to the directory where you saved the code.

4. Compile the code using the C++ compiler. For example, if you are using g++, you can compile the code with the following command:

   ```bash
   g++ ccwc.cpp -o ccwc
   ```
   This command compiles the ccwc.cpp code and generates an executable file named `ccwc`.

5. After successful compilation, you can run the program using one of the following formats:

   - To count lines, words, or bytes in a file:

     ```bash
     ./ccwc -l/-w/-c/-m fileName
     ```

     Replace `-l`, `-w`, `-c`, or `-m` with the desired option, and `fileName` with the path to the text file you want to analyze.

   - To read input from stdin and count lines, words, or bytes:

     ```bash
     cat fileName.txt | ./ccwc -l/-w/-c/-m
     ```

     Replace `-l`, `-w`, `-c`, or `-m` with the desired option and provide input through stdin.

6. The program will execute the selected operation and display the result on the terminal.

