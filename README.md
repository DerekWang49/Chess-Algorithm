# Chess Monte Carlo Simulation: King and Queen vs. King Endgame

## Overview
This project implements a **Monte Carlo simulation** to determine the optimal moves in a **King and Queen vs. King endgame** in chess. The goal is to simulate thousands of random game scenarios to analyze move effectiveness and strategy.

## Features
- Uses **Monte Carlo tree search (MCTS)** to evaluate game positions.
- Simulates **multiple endgame scenarios** to refine move selection.
- Written in **Julia** for high-performance computation.

## Installation & Setup
### Prerequisites
Ensure you have the following installed:
- **Julia** (version 1.9.3 or later)
- Required packages: `Pkg.add(["DelimitedFiles", "Pkg", "CSV", "JLD])`

### Running the Simulation
1. Clone this repository:
   ```bash
   git clone https://github.com/DerekWang49/Chess-Algorithm.git
   cd Chess-Algorithm
   ```
2. Run the simulation script:
   ```bash
   julia main.jl
   ```

## Methodology
Monte Carlo simulations work by:
1. **Randomly simulating** thousands of game sequences from a given board position.
2. **Tracking move outcomes** to estimate which choices lead to faster wins.
3. **Refining move selection** by iterating over multiple simulations.


## Future Improvements
- Give the user the option to manually play through an episode with their own move choice, while being able to view the policy for the given position

## Contributing
Contributions are welcome! Feel free to submit issues or pull requests.

## License

This project is for demonstration purposes only, intended for review by potential employers. All rights to the code and content are reserved by the author.

You may:
- View the project to evaluate my skills and work.

You may not:
- Modify, distribute, or use the code for commercial purposes without explicit permission.

This project is provided "as is", with no warranty of any kind.


---
*Created by [Derek Wang](https://github.com/DerekWang49)*

