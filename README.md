# AI_sokoban
  The game is in the form of a square board. There are a number of squares pushed to the destination (the number of target cells is exactly equal to the number of squares). Can only push blocks one at a time, and cannot pull, and cannot push a sequence of two or more blocks.
  
  The square is stuck to the wall if it is pushed close to the wall and both sides of the wall are corners. Since the block cannot be pulled back, it is considered lost, it cannot be brought to the destination unless the destination is exactly on the edge of the wall. Sticking to the wall is a case to avoid when playing.
  
  To move the character, you use the 4 arrow keys to navigate to push the crates into the correct position of the dots.
  
  ![v](https://user-images.githubusercontent.com/106755542/192467632-778a01e7-1b7b-4329-9282-77c82dc787b6.jpg)
  
  The Sokoban game can be viewed as a search problem by pushing the squares to the destination. And in this problem, we will solve it by 3 algorithms: BFS, DFS, UCS.
  
  The start state is the state when you initialize and enter that level and is determined by the game developer.
  
  End state is the state where all square boxes have been pushed to the destination.
  
  The state space is all the positions in the game frame.
  
  Valid actions are actions such as when going to the edge, it is not allowed to go forward but backward or can go up and down as long as the front is not a border and the square cannot be walled if it is blocked push close to the wall where both sides of the wall are corners. Since the block cannot be pulled back, it is considered lost, it cannot be brought to the destination unless the destination is exactly on the edge of the wall. Sticking to the wall is a case to avoid when playing.
  
  Progression function: is the next action but that action is not finished.
