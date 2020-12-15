# AgentBasedModel2
2nd asssignment for the Leeds programming module
# AgentBasedModel2

2nd Asssignment for the Leeds Programming for Social Science: Core skills module

This repository holds all of the files and information required for the Planning for Drunks ABM.

 

## Basic algorithm:

1.      Assign each drunk a house number from 10 to 250 before leaving the pub. For example, drunk number 20 will have to reach house 20

2.      Move drunks left/ right/ up/ down randomly

3.      When each drunk reaches the correctly numbered house, stop movement and continue process with other drunks

4.      For each step of each drunk, add one to the density map for that point

5.      Stop when all  drunks are home


## Instructions to run the code

To run the code, a suitable python software must be installed. The model was built using the IUD Spyder, which can be downloaded from the Anaconda navigator.

Both the .py files (modelfinal4.py and drunkagent7.py) need to be saved in the same folder. Ensure the raster file 'drunk.txt' is saved in the same directory as the agent and model files. The file must be saved as 'drunk.txt', as this is the name used to open the file in the code.

This file holds information about the town plan, which is used to show the pub point and houses. The file is laid out at one line per image line, from the top left to the bottom right of the file. The pub is represented by 1's, the house numbers 10- 250, and the empty space by 0's.


Before running the code, in the console, run '%matplotlib qt' to show the figures in a separate window. After doing so, you can run modefinal4.py, which will call the drunkagent7.py file and execute the model.

## What to expect

Once the model has run, 2 Figures will be produced. The first is a map of the town, titled 'Townplan' showing the houses and the pub in white, against a black background. The coloured dot shows the agents at the starting pub point.

Figure 2 is a density map showing the drunks at their homes. The lighter the colour the more drunks have walked over this point.

The density map will also be saved to a file as text. It will be called 'density.txt' and can be found in the directory the original files were saved. The values will change every time the model is run, representing the movement of the drunks.

Text will also be printed to the console, detailing the number of drunks who have reached home and then stating when all drunks are home
