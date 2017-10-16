# ZMaze
Application to study and creation and solution of mazes, ported from the JMaze app.  Will be written in WinRT C# with as much XAML and .NET shoved in as I can dream up.  Alterier motive is to use
this as a study base for MVVM.

## NOTE: 10/16/2017
After study of WPF and WinRT found that simple 2D graphics, such as DrawLine, are not possible in these apps. What I really need is to use DirectX or SharpDX.  But, I'm just not of a mind to learn that
right now. So, I'm checking in what I have and put this on the back burner for later.  I'll go over to my C# Maze app which using Forms (which allows simple 2D Graphics) and piddle with that.

# Requirements
* Maze will be a 2x2 grid of cells.
* The number of cells in x and y will be user defined
* Each cell will be square.  The number of pixels in x/y will be user defined
* The app will implement multiple algorithms defined at https://en.wikipedia.org/wiki/Maze_generation_algorithm and http://www.astrolog.org/labyrnth/algrithm.htm
* For algorthms which require the user to select a starting cell, the starting cell can be selected manually or randomly.
* The entrance and exit can be selected manually or randomly
* The x or y coordinate of the entrance and exit cell must be either north, south, east, west.  Implying that the entrance/exit is on the outer edge of the Maze
* The user can create the maze which updates the display after the maze has been created, or create the maze with animation, which means the display animates the carving out of the paths
* An option will be provided to solve the maze
* An option will be provided to print the maze
* A maze can be saved/loaded from a file containing multiple mazes.
* A control will contain the name of all saved mazes allowing the user to recall a previously created Maze
* The name of mazes will start with Maze-1 with the number incremented as new mazes are created.
* An option will be provided by which a maze can be deleted, removed from the collection
* An option will be provided by which the user can view a 2D top view of the maze and/or a 3D "in maze" view of the maze
* control keys will be defined by which the user can walk through the maze.  A marker will show the users current location

# Implementation Diary

### 10/13/2017
* ~~Convert from WPF to WinRT.  WPF doesn't seem to have simple primitive drawing functionality. Might want to revisit when I look at DirectX ~~
* Create a class for the walls
  * in the display panel, learn how to draw primitive 2D lines and shapes
  * create a wall and add it to a list
  * code to display the wall
  * display the walls  

* Add controls to the control panel (see JMaze)
  * clean up control display, 
    * add margins and paddings
    * parameterize the control sizes
	* create a template for the buttons
  * disable controls currently not implemented
* Create classes for the cells
* create the cells and walls for the grid. 
  * Save in dictionary
  * display 2D maze grid
  * create the maze
  * animate create the maze
* Create data binding for and implement the controls

### 10/13/2017
* ~~Add controls to the control panel (see JMaze)~~
  * ~~create raw controls~~

### 10/12/2017
* ~~Split the layout into a controls panel and display panel~~

# ZMazeWPF
Application to study and creation and solution of mazes, ported from the JMaze app.  Will be written in WPF C# with as much XAML and .NET shoved in as I can dream up.  

# Requirements

# Implementation Diary

### 10/13/2017
* Add controls to the control panel (see JMaze)
  * ~~create raw controls~~
  * clean up control display, 
    * add margins and paddings
    * parameterize the control sizes
	* create a template for the buttons
  * disable controls currently not implemented
* Create classes for the walls
* Create classes for the cells
* create the cells and walls for the grid. 
  * Save in dictionary
  * display 2D maze grid
  * create the maze
  * animate create the maze
* Create data binding for and implement the controls

### 10/12/2017
* ~~Split the layout into a controls panel and display panel~~

