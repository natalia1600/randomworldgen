# Bee Game (Random Worlds) 🐝 🧑🏻‍🌾

A 2D tile-based world exploration engine that generates and renders pseudo-random worlds.

## Description

The goal of the game is to reach the tomato and avoid being stung by bees along the way.

Game includes saving and loading capabilities, a 2D user interface with dynamic tiles, and a pseudo-random map generator. When loading a game from a previous session, a sped-up playback of previous actions taken will display before the game starts up again. The map layout is guaranteed to include some randomly sized/placed "rooms" and "hallways". Player cannot move outside of the rooms/hallways. To start a new game, you must enter a seed number when prompted. If you choose the same seed in future playthroughs, the map layout will be the same. Bees are randomly generated and move throughout the map with every few steps taken.



## Usage

To start the game, run the main method of the Main class. Users can provide the program a command line argument, describing how they want to generate the random world and what exploration they wish to complete, in which case, Main.main calls the Core.Engine.interactWithInputSting(String s) method. When running `Core.Main.main` with an input string, the format of the command argument should be `-s inputString`, where `inputString` is the input of `interactWithInputString()`. If no command line argument was provided, the user wants to interact with the program using a GUI menu and exploring the world using the keyboard, in which case `Main.main` calls the `Core.Engine.interactWithKeyboard()` method.


