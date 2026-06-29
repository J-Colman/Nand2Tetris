
# Project 2 - Boolean Arithmetic

26/06/2026 - Joshua Colman

---

This is the second Project in the Nand2Tetris series I am working through.

This Chapter began by explaining binary as a mathematical concept (base 2) and how to represent positive and negative integers in this format, then went on to show, through visualisations and methods, how to add and subtract binary sequences, before introducing the core chips we would build our Arithmetic Logic Unit from: the half-adder, full-adder, 16-bit adder and incrementer. As in the previous chapter, these chips are built from the smaller, simpler chips I had built previously, which themselves are built from logic gates and transistors.

The ALU took a little while to decipher. Originally I built it by simplifying the boolean algebra from the table having forgotten the Multiplexer and Demultiplexer existed, so it was composed of fundamental logic gates and completely overcomplicated. Upon remembering these chips existed, the task became vastly easier and the path to implementing the ALU became clear.

In a note at the end of the chapter, the authors highlighted the inefficient implementation of the current 16-bit adder and suggested an improved version: the carry look-ahead adder. This got me interested in what other variations of the adder were out there, so in addition to the Add16 16-bit Adder this project includes these exploratory adder variants:

- RCA4/RCA16: Ripple Carry Adders demonstrating serial propogation.
- CLA4/CLA16: Carry Look-ahead Adders demonstrating generate/propogate carry logic.
- CSel4/CSel16: Carry Select Adders demonstrating parallel precomputation.

These variants are included for comparison and learning purposes only.

As before, I also set up a dedicated project Github workflow to test all the chips implemented.