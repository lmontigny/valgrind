# valgrind

## Commands
gcc -O0 main.c -masm=intel  -fno-asynchronous-unwind-tables -g
valgrind --leak-check=yes ./a.out
valgrind --tool=memcheck --leak-check=yes --show-reachable=yes --num-callers=20 --track-fds=yes


## OUTPUT

# Process ID:
==16336== HEAP SUMMARY:

# Lost data:
==16336== LEAK SUMMARY:
==16336==    definitely lost: 40 bytes in 1 blocks

