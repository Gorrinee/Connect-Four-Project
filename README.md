# Connect Four Project
This Python project imitates the "connect four" board game. 
There are 3 different set ups for this game, so you can chose to play against a friend (player vs player mode), against a computer that makes random choices or against a computer with an AI algorithm. 

## Table of contents
* [General info](#general-info)
* [Screenshots](#screenshots)
* [Technologies](#technologies)
* [Setup](#setup)
* [Game Modes](#game-modes)
* [Code Examples](#code-examples)
* [Status](#status)
* [Contact](#contact)

## General info
There are 4 files in this project, each creating a different part of the game. 

The first one creates a board for the game, the second one creates a player, so that _you_, as a player, could make your move. Third one, the "Game" itself, imitates the process of taking turns to play the game, and the last one creates an AI player, that makes a move consciously, predicting your best move. 

The algorithm of this AI player is based on recursion and searching for the best move with the highest "score" of winning. In other words, each move the computer counts the score for each column based on the player's best move. 
There are also two parameters that you can chose for the AI Player: first one indicating how it will make its move if the chances of winning for two columns are the same. In this case you have three modes: always chose right column, left column, or chose it randomly. The second parameter, which is the number, shows how many steps ahead the computer will think through. 

The code also takes into account the borders of the board, so that, like in a real board game, you count't win if you had 3 checkers in a first row in the right corner of the table and 1 on the same row but in the left corner. 


## Screenshots
![Example screenshot](ConnectFourExample.png)

An example of a finised game where AI Computer Players wins. 


## Technologies
* Python - version 3.6.2

## Setup
Download all 4 files and run Module from the last file - *AIPlayer*. Enter the code line chosing one of the modes, as shown in Code Examples further below and start playing! 

## Game Modes
* Player vs Player  
* Player vs Random Player 
* Player vs AI Player

## Code Examples
Here are some examples of how one can start a game in Python Shell:

* Player vs Player mode 
`connect_four(Player('X'), Player('O'))`
* Player vs Random Computer 
`connect_four(Player('X'), RandomPlayer('O'))`
* Player vs AI Player
`connect_four(Player('X'), AIPlayer('O', 'RANDOM', 5))`, 

where the second parameter of the AI Players indicates how it makes a decision when the odds of winning is the same for 2 columns (choices are: 'RANDOM', 'RIGHT', 'LEFT') and the third parameter is the number of moves it thinks ahead. 

## Status
Project is: _finished_

## Contact
Created by Ekaterina Gorbunova - feel free to contact me at eginfo@bu.edu!
