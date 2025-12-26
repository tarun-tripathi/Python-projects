## Project Title: Snake Water Gun Game

This project implements a simple game of **Snake Water Gun** against the computer. It is a logic-based variation of the classic Rock-Paper-Scissors game, designed to demonstrate Python's conditional logic and numerical mapping.

---

### Description

The game allows a user to play against a computer that randomly selects its move. The core logic translates user input into numerical values to determine the winner based on the differences between the choices.

### Technologies Used

* **Python 3**: The core programming language used.
* **Random Module**: Used to generate the computer's choice.
* **Jupyter Notebook / Google Colab**: The environment used for development and execution.

---

### Game Rules

The game follows a specific hierarchy to determine the winner:

* **Water** drowns **Gun**: Water wins against Gun.
* **Gun** shoots **Snake**: Gun wins against Snake.
* **Snake** drinks **Water**: Snake wins against Water.
* **Draw**: If both players choose the same item, it's a draw.

### Key Features

* **Numerical Mapping**: Uses a dictionary to map choices to values (`w: -1`, `g: 0`, `s: 1`).
* **Refined Logic**: Instead of long `if-else` chains, the game uses the mathematical difference (`computer - you`) to identify outcomes.
* **User Interaction**: Takes real-time input from the user via the console.

---

### Logic Summary

The game determines the winner by evaluating the value of `computer - you`:
| Outcome | Numerical Difference (`computer - you`) |
| :--- | :--- |
| **You Win** | `-2` or `1` |
| **You Lose** | `-1` or `2` |
| **Draw** | `0` (when `computer == you`) |

