# TETRIS
A simple game where we apply what we learnt in class to practice the concept of OOP.

In this project, we use the Apache Net Bean IDE thanks to its beginner friendly GUI design. 

# To do list
 * Create the board game
 * Draw block on the board
 * Add block color
 * Make the block fall down
 * Spawn new block
 * Moving, rotating block on key press
 * Clear complete rows and add score
# Requirements
 * Java
 * Java Swing
 ---
 # Board game
 First, we create the game board by using JPanel, then we divided it into smaller cells base on the formula below.
 
 ![image](https://user-images.githubusercontent.com/52684784/170531720-a78f9f77-d865-4352-a5c3-d117951f5b68.png)
 # Drawing Block 
 After creating the board, now we need to draw the shape(tetrominoes) inside it.
 There are 7 tetrominoes in total, each of them will have different shape and color to distinguish.
 
 ![image](https://user-images.githubusercontent.com/52684784/170532176-af0e42d7-e8be-4d5b-827c-bd0361053e7c.png)
 
 Each tetrominoes will be stored in a 2d array with values 0, 1 where 1 is colored cell and otherwise.
 
 ![image](https://user-images.githubusercontent.com/52684784/170536852-7fd7791d-2aae-4706-9948-4323bbec6fc0.png)
 
 The output is something similar like this 
 
 ![image](https://user-images.githubusercontent.com/52684784/170541897-8541c3e1-042b-4b1d-b70c-f8e175f17076.png)
 # Make block fall down
 With the block spawning at the middle top of game board, now we need to make them fall down by 
 printing its postion after a fixed timestep and delete the previous one.
 
 So the process is: **print-wait-delete-print**

 
![image](https://user-images.githubusercontent.com/52684784/170737184-b2143150-c182-4f1b-b2c6-7dccdaeaee07.png)
# Line removal
* First we need to find the completed line
* Remove it
* Shift down the lines above
