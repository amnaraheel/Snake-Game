"Snake-Game"
Gaming industry is a multibillion-dollar industry and has maligned the youth to itself. Being fresh CS students and having interest in gaming, we built a snake game using the practical knowledge of C++ GAINED IN Programming Fundamentals Lab classes.


"Libraries"
We used iostream for regular input-output functions, windows,h for mode(), setup(), draw(), input(), logic() functions and conio.h is necessarily for _kbhit((), _getch() functions.


"Variable"
- gameover to keep a check on game.
- width and height are constants which are used to set the size of the walls.
- choice for choosing among menu options.
- mood for choosing the mode.
- x and y for snake’s head position.
- fruitx and fruity for positioning of fruit.
- score for showing the score.
- tailx and taily for positioning of tail.
- ntail for the length of tail.
- eDirection for control


"Mood Function"
This function is for the wall mode off the game in which when the head of the snake collides with the wall, it is 
game over.

"Setup Function"
Here, we initialized the gameover to false, dir to stop. Though we can generate the snake anywhere, but we have 
generated it in the middle. And after generating the snake, we then generated the food at any random point but 
within the height and width of the wall

"Draw Function"
Here we just build up the wall boundary. Display the snake from head to tail and the fruit. The walls are shown 
by ‘#’ character, the snake’s body is shown by ‘o’ characters and the fruit by ‘*’.

"Input Function"
In the input function, we used switch statements and when the _kbhit() function occurs we just maintained the 
switch cases (w, a, s, d) and change the direction respectively. The x key is for closing the game.

"Logic Function"
In the logic function, we first initialized the tail. And after that, we switched the position of the snake’s body with 
its previous position. And after that, the program simply needs to implement the body according to the keyboard 
hit. Next, as this follows the concept of an open maze, so when it disappears at one side, it appears from the other 
side, so we kept in mind that once it touches the right wall it appears from the other left wall and vice-versa and 
same follows for the up and down walls. Next, the head touches the body, the game crashes. For the scoring 
system we added 10 points hen the head touches the food (their position becomes the same). And every touch
increases the score.

"Main Function"
The main boy calls all the function and has the instructions to show the main menu and give a response according 
to the user input.

"Input"
The user uses the prescribed keyboard keys to play the game:

- Keys:

*[W] = Up
*[A] = Left
*[S] = Down
*[D] = Right

"Output"
Using the keys, the user can toggle through the menu and navigate the snake to get food.
