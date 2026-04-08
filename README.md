# Module Selection Optimisation Using Binary Integer Programming
![Operations Research](https://img.shields.io/badge/Field-Operations%20Research-blue)
![Optimization](https://img.shields.io/badge/Method-Binary%20Integer%20Programming-green)
![Tool](https://img.shields.io/badge/Tool-Excel%20Solver-orange)
![Status](https://img.shields.io/badge/Project-Academic%20Case%20Study-purple)

## Project Overview

Academic planning often requires students to select modules while satisfying programme requirements and timetable constraints. Manual decision-making can become difficult when multiple restrictions and preferences exist simultaneously.

This project demonstrates how **Binary Integer Programming (BIP)** can be applied to optimise module selection while maximising student satisfaction.

The model was implemented using **Microsoft Excel Solver**, providing an analytical approach to decision-making under constraints.

---

## Problem Statement

Sophie, a final-year Finance student, must select **five modules** for the academic year while satisfying several requirements:

• Two compulsory modules must be taken  
• One industry module must be selected  
• Two finance optional modules must be chosen  
• No timetable conflicts are allowed  

In addition, Sophie has preference ratings for modules based on:

- interest in module content  
- lecturer effectiveness  
- schedule convenience  

The objective is therefore to **maximise total satisfaction while respecting all academic and scheduling constraints**.

---

## Optimisation Method

The problem was formulated as a **Binary Integer Programming model**.

Binary decision variables were used:

xij = 1 if module j is selected in time slot i  
xij = 0 otherwise

### Objective Function

Maximise total satisfaction:

Max Z = ΣΣ Rij xij

Where Rij represents Sophie’s preference rating for a module at a specific time slot.

---

## Model Constraints

The optimisation model includes the following constraints:

1. Exactly five modules must be selected  
2. Two compulsory modules must be taken  
3. Exactly one industry module must be selected  
4. Exactly two finance optional modules must be chosen  
5. No more than one module per time slot  
6. A module cannot be selected more than once  
7. Overlapping time slots cannot be chosen simultaneously  

These constraints ensure the solution is both **optimal and feasible**.

---

## Implementation

The model was implemented using **Microsoft Excel Solver**.

Key steps included:

• Structuring the decision variable matrix  
• Creating a preference rating matrix  
• Implementing the objective function using the SUMPRODUCT function  
• Encoding all academic and scheduling constraints in Solver  

Solver used integer optimisation techniques to search for the best feasible combination of modules.

---

## Results

The optimisation produced an optimal satisfaction score of:

**Z = 19.5**

The final solution satisfied all constraints:

• Exactly five modules selected  
• Mandatory modules included  
• One industry module selected  
• Two finance optional modules selected  
• No timetable conflicts  

This demonstrates how optimisation models can effectively support structured decision-making.

---
## Model Structure

![Model Structure](https://github.com/Olafare-analytics/module-selection-optimization/blob/main/images/model-structure.png?raw=true)

The optimisation model was implemented in Microsoft Excel using a matrix of binary decision variables representing module selections across time slots.

---

## Solver Configuration

![Solver Setup](images/solver-setup.png)

Excel Solver was configured to maximise the objective function while enforcing all academic and scheduling constraints.

---

## Final Optimised Solution

![Final Result](images/final-result.png)

The solver produced an optimal satisfaction score of **Z = 19.5**, satisfying all constraints including mandatory modules and timetable feasibility.

---

## Initial Model Result (Before Adding Overlap Constraints)

![Initial Result](images/initial-result.png)

The initial solution produced a higher score of **Z = 19.8**, but it contained timetable conflicts. Additional constraints were introduced to ensure a realistic and feasible solution.

## Key Insights

This project highlights several important insights:

• optimisation models provide systematic decision support  
• real-world constraints often reduce theoretical optimal values  
• careful constraint design is critical for realistic solutions  

The final solution balanced **optimality with feasibility**, illustrating the practical value of Operations Research techniques.

---

## Tools Used

• Microsoft Excel  
• Excel Solver  
• Binary Integer Programming  

## Skills Demonstrated

- Mathematical Optimisation
- Binary Integer Programming
- Operations Research Modelling
- Decision Analytics
- Excel Solver Implementation
- Constraint Modelling
---

## Possible Extensions

Future improvements to the model could include:

• multi-objective optimisation  
• workload balancing across semesters  
• implementation in Python using optimisation libraries such as PuLP or Pyomo  

---
## Repository Structure

## Author

Olafare Sikiru Olaniyi  
Operations Research & Data Analytics
