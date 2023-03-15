# Rule 1 - worst case

When analysing the big O for a program always look at the worst case scenario.



Image you have a program that loops through a list till it finds a particular string that matches with the given condition. If the string is found early you could break and stop operation of the loop, but with rule 1 you need to assume that the match will be met only at the end of the list. Hence irrespective of the position where the match happens the program is always O(n) where n is max length of list
