##Reinforcement Learning Group Project

Zach Wiesenthal, Madhumitha Govindaraju, George Gabricht

#Project Proposal

###Summary:

The main idea is to solve a maze in Minecraft. There are multiple ways to solve the maze, some easy (and slow) like walking around a big loop, some complicated like jumping up a staircase, and some nearly impossible like digging underground. The inputs of the program are the world it perceives and actions/movements given for the agent to take. The outputs of the reinforcement learning program are the actions it takes (looking around, walking, jumping, attacking). A possible application is in learning about navigation.

###Evaluation Plan:

The metrics used to evaluate performance for the maze depends on the time it takes to complete the course. The end is determined by a pressure plate. The faster the agent completes the course, the higher the score it will achieve. Walking around a big loop will likely reach the end of the course in 60 seconds, jumping can reach the end in 30 seconds, and digging underground can reach the end of the course in 20 seconds. Another metric we can use is the distance from the end pressure plate or the starting location. For example the agent will receive a higher score for moving 15 blocks towards the end pressure plate than only moving 5 blocks in a different direction.

We will use a timer and at the end of the timer (about 3 minutes) or if the agent reaches the pressure plate we will conclude that simulation and measure how close to the end the agent got. We can make sure that over time the agent gets closer to the end goal, and eventually that it reaches the end goal in faster times. There are multiple ways to solve the maze, the most complex way will be tunneling under an obsidian wall through cobblestone. If it somehow solves the maze this way it will get to the end in a very short time and that is our moonshot case.

###Goals:

Minimum Goal 1: Reach the redstone block at the end of the short hallway. • Minimum Goal 2: Reach the end pressure plate by any way possible. There is a simple but long outer path that it will likely take to reach this goal. • Realist Goal 1: Jump up and over the obsidian wall, at least 3 blocks up and 5 blocks towards end goal. • Realist Goal 2: Jump up and over the obsidian wall and reach the end pressure plate. • Ambitious Goal: Tunnel under the obsidian wall in a direct path to the end goal. This will be the fastest way, but also the least simple path since it must break blocks and jump up eventually.

###How To Run The Program:

The code exists in our "First Milestone" Folder.

First add the DoubleMaze folder to you Minecraft/run/saves folder.

Second, change the path on line 13 of BasicMaze.xml to the path on your computer that reaches Minecraft/run/saves/DoubleMaze.

Third, add the DoubleMaze.py and DoubleMaze.xml to your Python_Examples folder.

Then you must launch the Malmo Minecraft client with launchClient.

Then from another window run python BasicMaze.py.
