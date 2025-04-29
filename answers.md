# CMPS 2200 Assignment 5
## Answers

**Name:**Michael Baron






- **1a.**
  theta(log_n / log_d) = theta(log_d n)
comes from simplication of the height being (d^h+1 - 1 ) / (d-1) >= n 
- **1b.**
for delete, once swapping right most node, you may have to swap new root node down h times (h = height). however, for each level
- you would also have to look at d children, giving it a work of O(d * log_d n)
for insert, there could be at most h swaps to get the node to the top of the heap, where h is the height. this means that the work is also O(log_d n)

insert is more efficient since it only looks at its parrent, suposed to all of d children

- **1c.**
in Dijkstra's algorithm the bound for delete would be 
- O(d|V| log_d |V|)
- as you would to E edges, and check for V vertexes at each spot 
for insert it would be
- O(|E| * Log_d |V|)
giving the total combined function of 
- O(|E| * Log_d|V| + d|V| log_d|V|)
- **1d.**
d = |E| / |V|
- for n = |V| and m = |E|
- we know that to get both sides of the above equation from part c to have constant growth
- d must = m/n. if m = n^(1 + epsilon) then d = n^epsilon. so log_d n is constant growth at = 1/epsilon
- n*(m/n) * log _m/n n = m log_m/n n
- 


- **2a.**

  starting at 0:
  APSP(0,0,0) = 0
  APSP(0,0,1) = 0
  APSP(0,0,2) = 0
  APSP(0,1,0) = N/A
  APSP(0,1,1) = -2
  APSP(0,1,2) = -2
  APSP(0,2,0) = N/A
  APSP(0,2,1) = 1
  APSP(0,2,2) = -1
  
  starting at 1:
  APSP(1,0,0) -2
  APSP(1,0,1) = -2
  APSP(1,0,2) = -2
  APSP(1,1,0) = 0
  APSP(1,1,1,) = 0
  APSP(1,1,2) = 0
  APSP(1,2,0) = N/A
  APSP(1,2,1) = 1 
  APSP(1,2,2) = 0
  
  starting at 2:
  APSP(2,0,0) = N/A
  APSP(2,0,1) = -1
  APSP(2,0,2) = -1
  APSP(2,1,0) = N/A
  APSP(2,1,1) = 1
  APSP(2,1,2) = 0
  APSP(2,2,0) = 0
  APSP(2,2,1) = 0
  APSP(2,2,2) = 0

- **2b.**
since k = 2, APSP(i,j,1) = APSP(i,j,2) unless the latter is a smalelr number
this is becasue the shortest pair will already of been found unless the shortest pair is on the last step.

you cannot write APSP(i,j,2) with APS(i,j,0) and APS(i,j,1) for all values and be definitively correct. 

- **2c.**

- **2d.**

- **2e.**



- **3a.**


- **3b.**


- **3c.**
