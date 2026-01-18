# Dice Roller

Simple command-line dice roller that prints ASCII art for each die and the total.

## Requirements

- Python 3.8+

## Install (Windows / PowerShell)

```powershell
python -m venv .venv
.\.venv\Scripts\Activate
pip install --upgrade pip
Run
From the project folder (PowerShell):
.\.venv\Scripts\Activate
python `Dice%20roller%20program.py`
Recommended: rename Dice%20roller%20program.py to dice_roller.py and run:
python `dice_roller.py`
Usage
The program prompts: How many dice?:
Enter a positive integer (e.g., 3) and press Enter.
The script prints side-by-side ASCII dice for each rolled die and a final total: N.
Quick fixes & suggestions
Filename: remove spaces/percent encoding (rename to dice_roller.py).
Input validation: wrap int(input(...)) in try/except to handle non-numeric input and ensure value > 0.
Large counts: for many dice, consider printing in rows (e.g., 10 dice per row) to keep output readable.
Reproducible testing: optionally accept a --seed CLI arg and call random.seed() for deterministic rolls.
Graceful exit: catch KeyboardInterrupt to exit cleanly when interrupted.
Troubleshooting
ValueError on input: provide an integer or update the script to validate input.
No output: ensure you run the script with the correct Python interpreter and that the terminal is focused.
Misaligned ASCII: ensure a fixed-width font in the terminal (e.g., Consolas, Courier New).
