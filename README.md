# Nussinov-Algorithm
Implementation of Nussinov Algorithm in Python. 

The recursive cases: 
* Case 1: i and j form a complementary base pair
* Case 2: i is unpaired
* Case 3: j is unpaired
* Case 4: bifurcation

I implemented two different traceback steps both using a stack. 
* The first one only looks at the matrix from dynamic programming. It checks the recursive cases in the order of Case 2, Case 3, Case 1, Case 4. In some cases, it gives out incorrect base pairs by mistaking a bifurcation for a complementary base pair. 
* The second one makes use of backpointers. It breaks ties in the order of Case 1, Case 2, Case 3, Case 4. It always gives out correct base pairs. 
