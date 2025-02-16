# King and Queen vs King Chess Monte Carlo Simulation
This project uses Monte Carlo Simulation to determine the optimal move for white in a King and Queen vs King endgame in any position.
Thousands of "episodes" would be run to continually improve the model's current knowledge of best moves.
It would punish a move if the episode later resulted in a draw (stalemate or 50 moves) or reward the move if the episode later resulted in checkmate.
Each episode consists of a starting position and normal chess play from there. Black would have a random legal move.
White's move would be based on the policy that is passed in (list of best known move for each given position). 
Each position that results from a move is added to a list of positions for each position.
The reward/punishment is then applied to each of those moves


## Installation Instructions
This project uses the Julia Language, along with Jupyter Notebook. Both of these need to be installed for the program to work.
After downloading the file, open Jupyter Notebook and then the file

## Usage
Run all cells on Jupyter Notebook. Once the iterations are complete, you can type in a line of the following form: "println(episode(policy, 0, true, [[<whiteKingRowNum>, <whiteKingColNum>], [<whiteQueenRowNum>, <whiteQueenColNum>], [<BlackKingRowNum>, <BlackKingColNum>]])"
Example:
println(episode(policy, 0, true, [[6, 5], [8, 5], [3, 4]]), true)

## Features
Running the main program will save the known optimal move set for each legal position King and Queen vs King legal position.
There is an option as explained above to simulate an episode. Here are the parameters to pass in for episode: episode(policy, ϵ=0.05, board_display=false, position=nothing, outcome=false, move_reward=false). ϵ stands for error rate, so if you want a simulation based completely on the policy, you would select 0. To display the board, set board_display equal to true. If you want to run an episode without updating the policy, set outcome equal to true). move_reward is a diagnostic tool that can be kept as false.


## Acknowledgements
- Inspired by my love of chess :)
- Monte Carlo Simulations learned from IE 3013 at the University of Minnesota

## Contact
If you have any questions regarding the project, reach out to me at derek.m.wang2@gmail.com.
