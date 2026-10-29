# Lab 4: Informed Search (Heuristics and A*)
Name: Shahzad Sadiq
Roll_no: SU-92-BSAIM-F25-387
Subject: Artificial Intelligence Lab
Instructor: Rasikh Ali
## Files
- lab4_astar_audit.py : A* with a zero heuristic UCS control, heuristic audit and overestimate experiment (Tasks 1, 2 and 3)
- lab4_tests.py : edge case and heuristic quality tests
- outputs/ : captured output of every script
- Lab4_Report.docx : full report
## Setup
Python 3.8 or newer is needed. No extra packages are needed, only the standard library.
## Run
python lab4_astar_audit.py
python lab4_astar_audit.py 1
python lab4_astar_audit.py 2
python lab4_astar_audit.py 3
python lab4_tests.py
The number runs only that task. Without a number all three tasks run.
## Notes
- Graph: S: A(1), B(4). A: C(2). B: G(5). C: G(3). Start S, goal G.
- Heuristic: S 5, A 4, B 4, C 2, G 0. These are abstract time estimates, not measured distances.
- The queue orders entries by f, then g, then node name.
- A node counts as expanded only when its successors are examined. The goal is logged but not counted.
- Stale queue entries are ignored and counted separately.
- The UCS control uses the same code with h = 0 for every node.
- The overestimate experiment changes only h(C) from 2 to 10.
