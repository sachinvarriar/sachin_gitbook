# Rule 4 - Drop Non Dominant terms

Say you have a function that has 2 loops one of O(n) and another one of O(n^2) then we can calculate the total Big O notation which is O(n + n^2), but with rule 4 that says drop the non dominant term then we are forced to drop O(n) which is not significant in comparison to O(n^2). As a result the actual big O of this loop is O(n^2), as the focus is not only on time taken but scale. Time complexity is more about scale that actual time of execution.



