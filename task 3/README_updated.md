# Lab 3: Uninformed Search (BFS, DFS, DLS, IDDFS and UCS)
Name: Shahzad Sadiq
Roll Number: SU-92-BSAIM-F25-387
Subject: Artificial Intelligence Lab
Instructor: Rasikh Ali
## Files
- lab3_bfs_dfs.py : BFS and DFS with step by step traces (Task 1)
- lab3_depth_search.py : DLS and IDDFS with FOUND, CUTOFF and FAILURE (Task 2)
- lab3_ucs.py : weighted graph, UCS and BFS comparison (Task 3)
- lab3_tests.py : edge case tests (start equals goal, unreachable goal, cycle, negative cost)
- outputs/ : captured output of every script
- Lab3_Report.docx : full report
## Setup
Python 3.8 or newer is needed. No extra packages are needed, only the standard library.
## Run
python lab3_bfs_dfs.py
python lab3_depth_search.py
python lab3_ucs.py
python lab3_tests.py
## Notes
- Successor order is fixed left to right, which is the tie breaking order.
- Depth counts edges and the start node A has depth 0.
- Visit order includes the goal node.
- The C to G corridor is an added extension used only in the weighted experiment.
- Edge weights: A-B 1, A-C 5, B-D 4, B-E 1, C-F 2, C-G 7, E-G 1.
