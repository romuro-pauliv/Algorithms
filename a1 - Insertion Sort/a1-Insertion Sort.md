# Insertion Sort

Our first algorithm, insertion sort:

| I/O | Info |
|-----|------|
|**Input**| A sequence of $n$ numbers $\langle a_{1}, a_{2}, ..., a_{n}\rangle$
|**Output**| A permutation (reodering) $\langle a_{1}^{'}, a_{2}^{'}, ..., a_{n}^{'}\rangle$ of the input sequence such that $a_{1}^{'} \le a_{2}^{'} \le ... \le a_{n}^{'}$

The numbers that we wish to sort are also known as the __keys__.

We start with __insertion sort__, which is an efficent algorithm for sorting a small number of elements. Insertion sort works the way many people sort a hand of playing cards. We start with an empty left hand and the cards face down on the correct position in the left hand. To find the correct position for a card, we compare it with each of the cards already in the hand, from right to left.

Our pseudocode for insertion sort is presented as a procedure called __INSERTION-SORT__, which takes as a parameter an array $A[1..n]$ containing a sequence of length $n$ that is to be sorted. (In the code, the number $n$ of elements in $A$ is denoted by $length[A]$). The input numbers are __sorted in place__. The numbers are rearranged within the array $A$, with at most a constant number of them stored outside the array at any time. The input array $A$ contains the sorted output sequence when __INSERTION-SORT__ is finished.

> Figure 1.1 - The operation of __Insertion Sort__ on the array $A = \langle 5, 2, 4, 6, 1, 3 \rangle$.
<img align="left" src="https://github.com/romuro-pauliv/Algorithms/blob/main/a1%20-%20Insertion%20Sort/static/Insertion%20Sort.png?raw=true" alt="Insertion Sort" width="500"/>

Array indices appear above the rectangles, and values stored in the array positions appear within the rectangles. __(a)-(e)__ The iterations of the __for__ loop of lines __1-8__. In each iteration, the black rectangle holds the key taken from $A[j]$, whitch is compared with the values in shaded rectangles to its left in the test of line 5. Shaded arrows show array values moved one position to the right in line 6, and black arrows indicate where the key moved to in line 8. __(f)__ The final sorted array.
