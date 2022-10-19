0x11. C - printf
Team project created by:Michelle Wangari & Fiona Githaiga 
Description: 
Printf : Writes formatted output to stdout
function format string is a character string, beginning and ending in its initial shift state, if any. These arguments are placed using the percentage '%' operator
Format control string
The format control string consists of:
multibyte characters
These are copied to the output stream exactly as they occur in the format string. An ordinary character in the format string is any character, other than a percent character (%), that isn't part of a conversion specifier.
conversion specifiers
These cause argument values to be written as they're encountered during the processing of the format string. A conversion specifier is a sequence of characters in the format string that begins with “%” and is followed by:
zero or more format control flags that can modify the final effect of the format directive
an optional decimal integer, or an asterisk (*), that specifies a minimum field width to be reserved for the formatted item
an optional precision specification in the form of a period (.), followed by an optional decimal integer or an asterisk (*)

Specifier	Output
c	Character
d or i	Signed integer
s	String of characters
b	Binary Representation of unsigned integer
u	Unsigned integer
o	Unsigned octal
x	Unsigned hexadecimal integer
X	Unsigned hexadecimal integer (uppercase)
S	String with hex-ascii value replacing special chars
p	Pointer address
r	Reversed string of characters
R	ROT13 Translation of string

Format Arguments
If there are leftover arguments after processing format, they're ignored.

Format control flags
The valid format control flags are:
Flag	Description
-
Left-justify the formatted item within the field; normally, items are right-justified.
+
Always start a signed, positive object with a plus character (+); normally, only negative items begin with a sign.
space
Always start a signed, positive object with a space character; if both + and a space are specified, + overrides the space.
#
Used with o, x or X specifiers the value is preceeded with 0, 0x or 0X respectively for values different than zero.
0	
Left-pads the number with zeroes (0) instead of spaces when padding is specified (see width sub-specifier).

Files contained in this repository

main.h - contains type struct, standard libraries and custom prototypes.
_putchar.c- contains the putchar function
_printf.c - contains printf file
man_3_printf - contains man page
printf_37.c	Contains percentage print function.
printf_int.c	Contains decimal and integer functions.
printf_char.c	Custom function for char data type.
printf_sting.c	Function that calls string type variable.
printf_bin.c	Function that gets the binary
printf_oct.c	Functions that returns octal number.
printf_hex.c	Calls hexadecimal numbers (lowercase).
printf_HEX.c	Calls hexadecimal numbers (Uppercase).
printf_unsigned.c	Returns an unisgined data type.
printf_hex_aux.c	Auxiliar function for hexadecimal specific functions (lowercase).
printf_HEX_aux.c	Auxiliar function hexadecimal specific functions (Uppercase).
printf_exclusive_string.c	Returns a string and non readable characters are printed in hexadecimal numbers (Lowercase).
printf_srev.c	Returns a string in reverse.
printf_rot13.c	Returns a string in Rot13.
printf_str.c	Auxiliar functions such as strlen and strcpy.

Tasks required for this project
0. Write a function that produces output according to a format.
Handle the following conversion specifiers:
    c,s,%
1.Education is when you read the fine print. Experience is what you get if you dont
Handle the following conversion specifiers:
d, i
2.With a face like mine, I do better in print
Handle the following conversion specifiers:
b: the unsigned int argument is converted to binary
3. What one has not experienced, one will never understand in print 
Handle the following conversion specifiers:
    u,o, x, X
4. Nothing in fine print is ever good news 
Use a local buffer of 1024 chars in order to call write as little as possible.
5. My weakness is wearing too much leopard print.                     Handle the following custom conversion specifier
S : prints the string.
Non printable characters (0 < ASCII value < 32 or >= 127) are printed this way: \x, followed by the ASCII code value in hexadecimal (upper case - always 2 characters).
6.How is the world ruled and led to war? Diplomats lie to journalists and believe these lies when they see them in print
Handle the following conversion specifier: p
7.The big print gives and the small print takes away
Handle the following flag characters for non-custom conversion specifiers:
´+´ space ´#´
8.Sarcasm is lost in print
Handle the following length modifiers for non-custom conversion specifiers:
l, h 
Conversion specifiers to handle: d, i, u, o, x, X
9.Print some money and give it to us for the rain forests
Handle the field width for non-custom conversion specifiers.
10.The negative is the equivalent of the composer's score, and the print the performance
Handle the precision for non-custom conversion specifiers.
11.It's depressing when you're still around and your albums are out of print
Handle the 0 flag character for non-custom conversion specifiers.
12.Every time that I wanted to give up, if I saw an interesting textile, print what ever, suddenly I would see a collection
Handle the - flag character for non-custom conversion specifiers.
13.Print is the sharpest and the strongest weapon of our party
Handle the following custom conversion specifier:
r : prints the reversed string
14.The flood of print has turned reading into a process of gulping rather than savoring
Handle the following custom conversion specifier:
R: prints the rot13'ed string
15.*
All the above options work well together.
