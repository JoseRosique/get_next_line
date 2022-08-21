<a href="https://github.com/JaeSeoKim/badge42"><img src="https://badge42.vercel.app/api/v2/cl4qxms4g001609l49j835g66/project/2574183" alt="joslopez's 42 get_next_line Score" /></a>
# get_next_line
It is a function that reads a file and allows you to read a line ending with a newline character from a file descriptor. When you call the function again on the same file, it grabs the next line. This project deals with memory allocation and when to free and allocate memory to prevent leaks.</n>
MANDATORY PART
• Repeated calls (e.g., using a loop) to your get_next_line() function should let you read the text file pointed to by the file descriptor, one line at a time. 
• Your function should return the line that was read. If there is nothing else to read or if an error occurred, it should return NULL. 
• Make sure that your function works as expected both when reading a file and when reading from the standard input. 
• Please note that the returned line should include the terminating \n character, except if the end of the file was reached and does not end with a \n character. 
• Your header file get_next_line.h must at least contain the prototype of the get_next_line() function. 
• Add all the helper functions you need in the get_next_line_utils.c file. Because you will have to read files in get_next_line(), add this option to your compiler call: -D BUFFER_SIZE=n It will define the buffer size for read(). The buffer size value will be modified by your peer-evaluators and the Moulinette in order to test your code. 
• You will compile your code as follows (a buffer size of 42 is used as an example): cc -Wall -Wextra -Werror -D BUFFER_SIZE=42 .c 
• We consider that get_next_line() has undefined behavior if the file pointed to by the file descriptor changed since the last call whereas read() didn’t reach the end of the file. 
• We also consider that get_next_line() has undefined behavior when reading a binary file. However, you can implement a logical way to handle this behavior if you want to.
