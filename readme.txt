In order to assemble (you should have nasm and ld be installed):

Type in console:
nasm -f elf64 input.asm
nasm -f elf64 output.asm
nasm -f elf64 main.asm

It produces .o files

Link modules:

ld main.o output.o input.o -o program

Eventually we get file program
That can be run (on linux): ./program