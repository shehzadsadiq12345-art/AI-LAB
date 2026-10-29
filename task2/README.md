# Lab 2: Intelligent Agents & the PEAS Framework

- **Name:** Shahzad Sadiq
- **Roll Number:** 387
- **Subject:** Artificial Intelligence Lab
- **Submitted to:** Rasikh Ali

Smart classroom energy agent (Artificial Intelligence Lab).
All operating modes (ECO, COOL, WARM, IDLE) are simulated labels; no hardware is controlled.

## Setup

- Python 3.8 or newer. No third-party packages are needed.
- No credentials, data files or virtual environments are required.

## Run

```bash
cd lab2
python lab2_percepts.py   # reflex agent, 6-percept trace
python lab2_model.py      # stateful agent, full mode-transition trace
python lab2_check.py      # tests, reflex vs stateful comparison, noisy edge case
```

Captured outputs are saved in `output_percepts.txt`, `output_model.txt` and `output_check.txt`.

## Files

| File | Purpose |
|------|---------|
| `lab2_percepts.py` | Reflex `ClassroomAgent` and the 6-percept trace |
| `lab2_model.py` | Stateful agent (previous mode + send/no-send) and trace printer |
| `lab2_check.py` | Assertions for boundaries, transitions, empty room, noisy edge case |
| `Lab2_Report.docx` | PEAS specifications, classifications, comparison, trace, reflection |
| `output_*.txt` | Captured program output |

## Policy

- Empty room has priority: `ECO`.
- Occupied and temperature > 26 C: `COOL`.
- Occupied and temperature < 20 C: `WARM`.
- Otherwise (including exactly 20 C and 26 C): `IDLE`.

## Sources

The reflex agent and thresholds come from the Lab 2 manual (Section 2.4 / 2.5). The stateful extension is my own work.
