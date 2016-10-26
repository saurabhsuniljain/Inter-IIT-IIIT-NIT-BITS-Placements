#Online Round
1. **Problem Statement** : Here you've to find number of H,L,T,U in a NxN grid (contains only 0 and 1). Each pattern can be represented in form of 3x3 matrix and can be rotated in 90,180,270 degrees.

    H -   
          
          1 0 1    1 1 1
          
          1 1 1    0 1 0
          
          1 0 1    1 1 1
    
    L -   
          
          1 0 0
          
          1 0 0 and three more forms
          
          1 1 1
   
    T -    
          
          1 1 1
          
          0 1 0 and three more forms
          
          0 1 0
    
    U -   
          
          1 0 1
          
          1 0 1 and three more forms
          
          0 1 0

  **Sample Test Case**
  
  **Input** :
    
    0 0 1 1 1 0 1 0 0
    
    0 0 0 0 1 0 1 1 1
    
    0 0 0 0 1 0 1 0 0	
    
    0 0 0 0 0 0 0 0 0
    
    1 1 1 0 0 0 1 1 0
    
    0 1 0 0 0 0 0 0 1
    
    1 1 1 0 0 0 1 1 0
  
  **Output** : 1 1 1 1
    
    It is guaranteed that a valid pattern exists and two patterns are separated by boundary of one.

2. **Problem Statement** : Given  height of N*N buildings in form of NXN matrix and a ball can be assumed to be dropped from a building. Ball will fall on its neighbour having lowest height.
    e.g. ball from a[i][j] will fall on min(a[i+1][j],a[i-1][j],a[i][j+1],a[i][j-1]) and goes on falling.
    You have to find length of maximum path that can be traversed by ball.
    
    **Input** :
    
    3x3
    
    1 2 3
    
    4 8 9
    
    6 0 5
    
    **Output** : 4 (9->3->2->1) 
