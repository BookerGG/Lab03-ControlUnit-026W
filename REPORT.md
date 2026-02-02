### Part 1

Tests 1 - 4 all test immediate instructinons starting with addi, load word, store word, and then branch equal. The next ones are testing the register instructions add, subtract, and, or, nor, and less than.

### Part 2

The first difference is in the reg_dst signal with addi being 0 since it is immediate while add is 1 since it is register, so they have to be specified differently. Next is alu_op with addi being 00 since it is fixed while add is 10 so that it can figure out what operation it is going to perform. Last is alu_src with addi being 1 since it is immediate and add is 0 so that it can use two register values.