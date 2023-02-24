# Rule 3 - Different terms for inputs

You could have 2 loops that take different inputs in the same function. If the arguments are different and there are separate loops that operate on each of these arguments the big O becomes something like O(n + m).



This could also happen such that there are nested loops, in which case we end up with a O(n^2)

When you see nested loops the big O is O(n\*n) which is O(n^2)
