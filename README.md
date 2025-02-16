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


## Acknowledgements
- Inspired by my love of chess :)
- Monte Carlo Simulations learned from IE 3013 at the University of Minnesota

## Contact
If you have any questions regarding the project, reach out to me at derek.m.wang2@gmail.com.
