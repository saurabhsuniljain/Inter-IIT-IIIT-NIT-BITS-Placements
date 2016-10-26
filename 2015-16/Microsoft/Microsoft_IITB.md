#Online Round (30 Oct 2015)

**Platform** : Cocubes

**Format** : Two sections Aptitude and Coding.

## Aptitude - 15 MCQs (30 mins)

1. The number of leaf nodes in a rooted tree of n nodes, with each node having 0 or 3 children is:

  Ans : (2n+1)/3 (Geeksquiz question)

2. Fetch_And_Add(X,i) is an atomic Read-Modify-Write instruction that reads the value of memory location X, increments it by the value i, and returns the old value of X. It is used in the pseudocode shown below to implement a busy-wait lock. L is an unsigned integer shared variable initialized to 0. The value of 0 corresponds to lock being available, while any non-zero value corresponds to the lock being not available.
 
 `AcquireLock(L){
    while (Fetch_And_Add(L,1))
      L = 1;
  }
  ReleaseLock(L){
    L = 0;
  }`

  Ans :fails as L can take on a non-zero value when the lock is actually available (GeeksQuiz)

3. Unary operator - in c. //what to infer from bridge, can someone explain

  options: a) 165  b)170  c) 195   d) 209
  
  Ans??-- did someone get the ans for this? (How??) wasn’t there a condition like steps should be minimum? Otherwise it can go to infinity (going into a loop) or at least a condition like we can go only once on any block.

4. Linked List What is the output (Not remembering exact Questions)

5. Linked List What is the output (Not remembering exact Questions) 
    List was given 1-2-3-4-5-6-7-8;  Some operation on list and list was printed at last.

6. Question on Virtual Function: (What is output) 3 classes were given each overriding same function of base class.
    Array of base class storing objects of 3 classes. Then a call to functions made.

7. Question on Java Char Array, character stream. (What is output)

8. What is output of this C++ code: ( not remembering exact code) Conversion Operator overloading:

9. Question on C preprocessing : (Not remembering exactly)
  
  But was somewhat like this:
  edi
  }
  
  Options:a) 11, b) compile error , c).. , d)..
  
  doubt: what will while(s(90),4) do. I think s(90)=”90” right??


10. Questions on Structure pointers

11. Questions on Structure pointers

12. Consider a weighted complete graph G on the vertex set {v1, v2, ..vn} such that the weight of the edge (vi, vj) is 2|i-j|. The weight of a minimum spanning tree of G is: 
  
  (A) n - 1   (B) 2n- 2   (C) nC2   (D) 2                     (GATE CS 2006)
  
  ans: 2n-2

13. Consider the following array of elements. 〈89, 19, 50, 17, 12, 15, 2, 5, 7, 11, 6, 9, 100〉. The minimum number of interchanges needed to convert it into a max-heap is:

  a) 3    b) 4   c) 5   d) 2
  
  ans: 3


14. Not remembering

15. Not remembering

## Coding - 2 questions (1 hour)

1. Longest Even Length Substring: 
  
  **Problem Statement** : Given a string of digits. Find the length of longest even length substring such that the sum of left part = sum of right part. Return 0 if no such substring exists.
  
  **Example**: Given string 1523457. The longest even length substring will be 5234. So output = 4.
  
  ![alt text] (https://github.com/saurabhsuniljain/Inter-IIT-IIIT-NIT-BITS-Placements/blob/master/2015-16/Microsoft/Images-and-Raw-material/image29.jpg)
   
2. Minimum difference of subarray [TUG OF WAR]
  
  **Problem Statement** : Given an array of length n. Divide the array between two subarrays such that diff between sum of each subarray should be minimum. For even n: subarray lengths should b n/2 exact, for odd n: subarray lengths should be (n-1)/2 and (n+1)/2
  
  **Example** : Given array 5,6,11,13,14,25. Two subarrays: {5,6,25} and {11,13,14}.
  ![alt text] (https://github.com/saurabhsuniljain/Inter-IIT-IIIT-NIT-BITS-Placements/blob/master/2015-16/Microsoft/Images-and-Raw-material/image34.jpg)
