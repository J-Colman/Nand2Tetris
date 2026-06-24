
# Project 1 - Boolean Logic

24/06/2026 - Joshua Colman

---

This is the first Project in the Nand2Tetris series I am working through.

This first Chapter started at the very bottom, declining to go too far into the physics beyond semiconductors and voltage, but giving more than enough context to understand what is built on top, starting with transistors, which are wired together to create the fundamental logic gates, and then those too are wired together to create increasingly complex components.

The main deliverables of this Project involved describing and simulating these logic gates in a custom Hardware Description Language provided by the Nand2Tetris creators, by first constructing a NOT gate from the elemental NAND gate, which then allowed me to build the AND and OR gates, and then more complex components such as the Multiplexer and Demultiplexer, which route input or output, all built hierarchically from the gates before. The latter half of this Project then had me creating multi-bit variations (performing the same operation on multiple input bits) and multi-way variations (handling multiple bits at the same time) of these same components, enabling new functionality.

After confirming all these components functioned locally, I created a GitHub workflow that downloads the necessary software and checks each gate simulation functions as expected by comparing the truth table output of each simulated gate against a static file containing the correct truth table, providing visual and automated confirmation that this whole project is progressing successfully and functioning correctly.