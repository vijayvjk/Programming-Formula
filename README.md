# Programming-Formula
An Guide for competitve problem

## Paranthesis Validation:

1. Breaking the Problem into sub problems
   1. A paranthesis is valid only when a open braces meets its corresponding closing paranthesis. So need to find the logic of "corresponding closing braces"
      1. Solving the problem manually (*typically called bruteforce*)
            Keyword: Removing matched string using Linear search
         We usually use a for loop with index x1 as 1st pointer and another inner for loop  with index x2 as 2nd pointer. on first look, the first pointer is placed at 0th index and 2nd pointer is placed at x1+1th index. we have to move 2nd pointer until we find a pair.  Once a pair is found, we can remove them;
         This process will be repeated to each and every x1nth pointer does resulting in a worse case of o(n^2).
         If all the pairs are deleted, we can say its a valid paranthesis.
      
      2. Using Stack Datastructure:
         Keyword: Back tracking recent activities / back tracking recently occured value / matching a paranthesis
         In a stack dataStructure
