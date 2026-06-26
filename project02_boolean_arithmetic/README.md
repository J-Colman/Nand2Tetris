
# Project 2 - Boolean Arithmetic

26/06/2026 - Joshua Colman

---

This is the second Project in the Nand2Tetris series I am working through.

This Chapter began by explaining binary as a mathematical concept (base 2) and how to represent positive and negative integers in this format, then went on to show, through visualisations and methods, how to add and subtract binary sequences, before introducing the core chips we would build our Arithmetic Logic Unit from: the half-adder, full-adder, 16-bit adder and incrementer. As in the previous chapter, these chips are built from the smaller, simpler chips I had built previously, which themselves are built from logic gates and transistors.

The ALU took a little while to decipher. Originally I built it by simplifying the boolean algebra from the table having forgotten the Multiplexer and Demultiplexer existed, so it was composed of fundamental logic gates and completely overcomplicated. Upon remembering these chips existed, the task became vastly easier and the path to implementing the ALU became clear.

In a note at the end of the chapter, the authors highlighted the inefficient implementation of the current 16-bit adder and suggested an improved version: the carry look-ahead adder. This got me interested in what other variations of the adder were out there, so I did a small amount of research and came across this article comparing the performance of multiple adder variants using various metrics:

https://www.irjet.net/archives/V9/i10/IRJET-V9I10133.pdf

Two variants in particular caught my attention: the carry look-ahead adder mentioned by this project's authors and the carry select adder, an adder with notable latency benefits. I decided to extend the project and implement both of these chips, settling on using the carry select adder in my ALU chip.

As before, I also set up a dedicated project Github workflow to test all the chips implemented.