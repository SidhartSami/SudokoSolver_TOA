# 🧠 Sudoku Solver 

Author: Sidhart Sami (https://www.linkedin.com/in/sidhart-sami/)<br> 
Project Title: Sudoku Solver - Theory Of Computing <br>
Term: Spring 2025<br>
Institution: FAST National University of Computer and Emerging Sciences (FAST-NUCES), Karachi Campus<br>
Technologies: HTML/CSS <br>
Concept Used: Multi-Tape Turing Machine

---

## 📌 Overview

This project simulates a **Multi-Tape Turing Machine** designed to solve 9x9 Sudoku puzzles using a **backtracking algorithm**. Built with web technologies, it features an interactive UI, visual tape transitions, and a dynamic state diagram.

---

## ✨ Features

### 🎯 Interactive UI

* ✅ 9x9 Sudoku grid with fixed, filled, and active cells highlighted
* 🖱️ Step-by-step simulation of Turing Machine behavior
* ⚡ Instant solve option with fast backtracking
* 🌗 Light/Dark theme toggle
* 📱 Responsive design for various screen sizes

### 🧠 Multi-Tape Turing Machine

* **Main Tape:** Linear representation of the Sudoku grid
* **Fixed Tape:** Tracks the original puzzle values (immutable cells)
* **Backtracking Tapes:**

  * Position Tape: Stores coordinates where values were tried
  * Value Tape: Records values attempted during backtracking

### 🔁 State Diagram

* Visualizes the machine's logic:

  * `Scan`: Skip filled cells
  * `Try Value`: Attempt digits 1–9
  * `Accept`: Puzzle solved
  * `Reject`: No solution found
* Animated transitions and active state highlighting

### 🧩 Puzzle Options

* Load puzzles of varying difficulty:

  * Easy
  * Medium
  * Hard
  * Expert

---

## 🛠️ Technologies Used

* **HTML / CSS** – Structure & styling of UI
* **JavaScript** – Turing Machine logic, dynamic updates
* **SVG** – Smooth state diagram rendering
---

## 🚀 Installation & Running Locally

```bash
# Clone the repository
git clone https://github.com/your-username/sudoku-turing-machine-simulator.git

# Navigate into the project directory
cd sudoku-turing-machine-simulator

# Open in browser
open index.html   # macOS
# OR
xdg-open index.html   # Linux
# OR manually open it in any browser
```

No additional dependencies or build tools required.

---

## 🧪 How to Use

1. **Load a Puzzle**

   * Select difficulty (Easy/Medium/Hard/Expert)
   * Click **"Load Puzzle"**

2. **Control the Simulation**

   * **Step**: Advance one state transition
   * **Run/Stop**: Play or pause execution
   * **Reset**: Restore puzzle to original state
   * **Solve Immediately**: Apply fast backtracking algorithm
   * **Speed Slider**: Adjust simulation speed

3. **Track Progress**

   * Grid: Shows current puzzle state
   * Tapes: Display cell values, positions, and backtracking data
   * Diagram: Highlights the current Turing state

---

## ⚙️ Project Structure

```
sudoku-turing-machine-simulator/
├── index.html         # Main file with embedded CSS and JavaScript
└── README.md          # Project documentation
```

> 🔎 `index.html` includes:
>
> * Embedded `styles.css`: Theme styles, grid visuals, tapes, etc.
> * Embedded `script.js`: Turing logic, UI controls, and event handlers

---

## 🧮 How It Works

The simulator emulates a **4-tape Turing Machine**:

* **Main Tape**: Linear 81-cell representation of the Sudoku grid
* **Fixed Tape**: Marks immutable cells
* **Backtracking Position Tape**: Tracks current cell positions
* **Backtracking Value Tape**: Tracks values tried for each position

### 🌀 State Flow

| State       | Description                                       |
| ----------- | ------------------------------------------------- |
| `Scan`      | Skip fixed cells, move to empty ones              |
| `Try Value` | Try numbers 1–9 while checking Sudoku constraints |
| `Accept`    | All cells filled with valid values                |
| `Reject`    | Backtracked completely without finding a solution |

---

## 🌟 Future Enhancements

* 📝 Add custom puzzle input by users
* 📊 Animate tape movements and head position changes
* ⚡ Optimize the backtracking logic for performance
* 📖 Step-by-step explanation of transitions and constraints

---

## 📬 Contact

Got feedback or want to collaborate?

[📇 Connect on LinkedIn – Sidhart Sami](https://www.linkedin.com/in/sidhart-sami/)

© 2025 Sidhart Sami – All Rights Reserved.
