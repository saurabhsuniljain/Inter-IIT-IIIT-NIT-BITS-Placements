#Online Round
**Single coding question** :

**Problem Statement** : Given n*n matrix (n<=100), where some cells will have mirrors of one of two types. Type 1 : “/” and Type 2 : “\”. These mirrors will reflect light by 90 degree. A single ray of light enters at (0,0). You have to find out the count of the number of reflections on mirrors before the ray leaves the grid.

**Solution** : store current direction (4 directions possible). If current cell has mirror, update direction correspondingly and increase reflection count. Also keep updating x, y coordinates given direction. When current coordinates reach out of grid print the count.
