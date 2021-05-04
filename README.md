# ARM-thumb-simmy
This repository was created for our Computer Architecture class cpe315 at Cal Poly SLO. The goal of this project is to create an ARM Thumb Simulator.

Contributors: Laura C., Diego G., Ryan N., and Yuya S.
For: Maria Pantoja

We have been provided with some support code that is written in ARM that our simulator is supposed to eventually run.
Once completed, our simulator will support the following instructions:
## Tasks
The simulator should handle a subset of the ARM Thumb instruction set. The 
"Shang" benchmark on which you will do measurements has the following 
instructions that you must support: 

  * push
  * pop
  * sub (sp minus immediate)
  * sub (immediate)
  * sub (register)
  * add (sp plus register)
  * add (sp plus immediate)
  * add (register)
  * add (immediate)
  * cmp (register)
  * cmp (immediate)
  * mov (immediate)
  * mov (register)
  * str
  * strb
  * stmia
  * ldr
  * ldrb
  * ldr (literal)
  * ldmia
  * b (unconditional)
  * bcc
  * bcs
  * beq
  * bge
  * bhi
  * ble
  * bls
  * blt
  * bne
  * bl
  * lsl (immediate)
  * neg.

Our tasks are as follows:

Complete the simulator so it successfully runs the fib and Shang benchmarks
(details below). The simulator, as provided, implements only a handful of 
instructions. You need to add support for other instructions.

You also need to collect statistics on the benchmark that you run to answer 
the questions in the writeup. Please measure dynamic (runtime) statistics for:
  * Number of instructions
  * Number of Memory Reads and Memory Writes (push, pop, ldm and stm count 1 for each register handled by the instruction).
  * Number of Conditional Branches, both forward and backward, taken and not taken in each direction. Do not include unconditional branches (including procedure calls or returns) as branches.
  * Cache performance. For a 256-byte direct-mapped cache, what is the best block (line) size in bytes? You could choose to have 64 entries in the cache of 4 bytes each, or instead 1 entry of 256 bytes, or anything in between. What has the best hit rate?

You will measure statistics for different optimization levels of the Shang 
benchmark. Example outputs from the instructor's simulator for the fib and 
shang benchmarks are included in the sample outputs directory. 
