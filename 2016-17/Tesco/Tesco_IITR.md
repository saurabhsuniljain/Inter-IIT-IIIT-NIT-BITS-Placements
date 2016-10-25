#Online Round
**Format** : 2 coding questions, 90 mins
##Questions
1. Police and Theives :
    
    **Problem Statement** : 
    
    Given a n*n matrix with either a ‘P’ police or ‘T’ thief in each cell, a police officer can only catch a thief in its row who is in the range k(given) of the police officer in either direction.
    Find out maximum no. of thieves that can be caught.
    Each police officer can catch up to 1 thief only.
    
    **Example**:
      
      1 
      
      n=3 k=1
      
      P T P
      
      T P T
      
      T T P
    
    Solution is 3. Every police officer can catch a thief.
    
2. Manjhi: The mountain man
    
    **Problem Statement** :
      
      Manjhi and the dragon with power ‘p’ is separated by an some rocks (array H[n]), with labels 1,2 or 3. 
      Every rock (but not the 1st and the last, as then the dragon will be able to attack the village) must be broken to fight with the dragon. 
      Breaking a rock decreases power of dragon by the factor( H[i] ^ H[i-1] ^ H[i+1]) and takes H[i] power of manjhi to break it. Manjhi wants to minimize the power of dragon after breaking all the stones except 1st and last. Can you help Manjhi??

##Solutions
1. Approach : Can be done in O(n) by using two pointers. 
    1. Prepare two arrays to store indices of police and thief. 
    2. Now use two pointers to mark current police and current thief, initialized to 0. 
    3. 
        1. If thief is in range of police, increment both police and thief pointers and increase count by 1,
        2. else if thief is on left outside the range increase thief pointer, 
        3. else increase police pointer. 
    4. Repeat till both police and thief pointers are less than X.end() [X can be police or thief vector containing, their indices].

    Process each row independently.
    
    **Overall Complexity** : O(n^2) ( 1 <= N <= 1000) [for whole matrix, O(n) for each row.]
2. Hint: 
    Use dynamic programming. Similar to matrix chain multiplication
    Think why greedy won’t work.??
