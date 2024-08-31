# Python-Robotics
This project integrates machine learning and robotics to build a fully functional robot using GoPiGo3 and Raspbian for Robots in a Raspberry PI while using Python as the instructing programming language. 

Cyber-Random-Rover in simple terms is a robot that uses a program that automates the GoPiGo with a memory that allows it to remember instructions. This robot drives around freely with no lines to follow, it does not just drive around in straight line but in random directions and straight lines for a while sometimes makes U-turns. The Cyber-Random-Rover has a memory so that it remembers the instructions that were processed. When the robot has finished processing all the movements it then performs all the movements backwards. The first instruction becomes the last instruction to be processed.

All this is made possible by the program I programmed using the Jupyter Notebook interface, which I access through the IP address 10.10.10.10 after connected to the Wi-Fi of DexterOS designed for the GoPiGo3. 
These are the following files I use:
1)	Python file (cyber_rover.ipynb)
2)	CSV file named (saved_directions.csv) 
3)	Text file named (live_memory.txt)

Python file 
Cyber_rover.ipynb is the backbone of the robot’s purpose. This file contains code that generates the random directions the robot wants to go; the user only specifies how many directions/steps the robot should take. Not only that but this file is also responsible for creating the csv and the text file.

CSV file
Saved_directions.csv is responsible for saving the programs generated directions so that the python file can retrieve to run them on the robot or retrieve to reverse them then run them on the robot.

Text file 
live_memory.txt is the robot’s live memory. Its purpose is to act as the storage place for the python program. The robot’s activities must be consistently saved so that if the robot runs out of batteries during the run, next time it is started it needs to be able to start from its last instruction before it shuts down. I chose the text file because it is the most flexible file to store and retrieve and importantly to iterate through the file.

					
					                   GoPiGo3 Robot
        Robot’s Right Side                Disconnected (Green)     Connected (Blue)                   Robot’s Left Side

       
