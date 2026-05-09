# Bubble Sort in MARIE Assembly
 
Bubble sort implemented in MARIE assembly language — no loops, no array indexing, one register. Every comparison, swap, and branch is done manually at the instruction level.
 
## Why It's Interesting
 
MARIE has no loop construct, so all 4 passes are fully unrolled. Comparisons are done by subtracting two values and checking if the result is negative (`Skipcond 000`). Swaps require a 3-step temp variable since there's only one accumulator.
 
## How to Run
 
1. Open [marie.js.org](https://marie.js.org) in your browser
2. Load `bubbleSort.mas` and assemble
3. Enter 5 integers when prompted — outputs them sorted ascending
## Example
```
Input:  5 3 8 1 4
Output: 1 3 4 5 8
```
 
