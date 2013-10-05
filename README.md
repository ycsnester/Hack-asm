Hack-asm
========

LISP IN SUMMER PROJECT:A compiler for the book &lt;The Elements of Computing Systems> 's Hack machine

This books introduces how to build a simple machine from Logic Gates and Flip-Flop.

In chap4 and chap6,it shows us this Hack-machine's language, there are 2 kinds of instruction:

1. A instruction
   to set A-register a value by @number.( @12 mean set A-reg to be 12)
2. C instrcution
   compute a result and store it:

   D=D+1
   
   means add 1 to value of D-register and store it in D-reg.
   (There are only two A-D registers in Hack-machine)

   or jump to an address which is specified by A insrtuction previousluy.
   such as:
   
   @40
   D-1;JGT
   
   means if D-1 's result is > 0 then jmp to (set program-counter) ROM[40].
   
Useage


1.you shoule write Hack-asm code in ABCED..not abcde.

2.I didn't make ' (symbol) ' instruction legel.

3.no symbol is allowed to mark address (sorry).


4.build /home/hack Directory

5.write down your code in /home/hack/source.asm.

6.run clisp *path*/asm_compiler.lisp.

7.then you get hack file in /home/hack/hack.
8.if you find NIL in hack file,you may typed the wrong asm code.
For more infomations, 

please see the excellent book <The Elements of Computing Systems>




   
