# Exploring Statistical Computing

## Project Contributors
|       Name        |      Student ID |Phone Number|
|-------------------|-----------------|------------|
| Virginia Wamaitha | BSCCS/2024/32333|0726157565  |
| Chemutai Sylvia   | BSCCS/2023/65519|0703198060  |
| Angeline Kipkemei | BSCCS/2023/52628|0721727646  |
| Edwin Meiteikini  | BSCCS/2024/44160|0746075436  |
|  Joyce Njeri      | BSCCS/2022/52454|0768586538  |
| Samuel Otieno     | BSCCS/2019/51244|0759566557  |
|Mary Wanjiku Maina | BSCCS/2023/44160|0705492382  | 



## What's This About?

This repository showcases practical examples across three programming languages commonly used in statistical computing: **Julia**, **Python**, and **R**. You'll find basic data operations in the `BasicsOfData/` directory, plus a deeper dive into arrays and data frames under `Arrays and DataFrames/`.

The R lesson covers:
- Working with arrays and matrices
- Building and manipulating lists
- Understanding data frames
- Basic modeling and visualization

We've also included a Python equivalent that produces identical outputs.

---

## Before You Begin

Make sure you have:
- A Linux environment with bash
- Julia (check with `julia --version`)
- Python 3.11 or newer
- R (only needed if running R scripts)

---

## Running the Examples

### Python

**Setting up the environment:**
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

**Execute the basic script:**
```bash
./.venv/bin/python BasicsOfData/math_operations.py
```

**Run the arrays and data frames lesson:**
```bash
./.venv/bin/python "Arrays and DataFrames/arrays_and_data_frames.py"
```

Generated plots will appear in the `plots/` folder:
- `allegheny_actual_vs_predicted.png` (requires successful dataset download)
- `illiteracy_vs_frost.png`

> If the CSV download fails, the Pennsylvania regression section will be skipped, but everything else runs normally.

---

### Julia

**Execute the script:**
```bash
julia BasicsOfData/math.operations.jl
```

**Keep in mind:**
- Don't name variables after built-in functions like `sum` or `names`
- Julia requires explicit broadcasting—arrays won't auto-recycle like in R

---

### R

**Basic operations:**
```bash
Rscript BasicsOfData/math_operations.R
```

**Arrays and Data Frames lesson:**
```bash
Rscript "Arrays and DataFrames/Arrays and Data Frames.r"
```

This lesson walks through:
- Creating and indexing arrays/matrices
- Matrix operations (transpose, determinant, inverse, solving systems)
- Working with lists and named elements
- Data frame manipulation and summary stats
- Linear regression on housing data
- Eigenvalue decomposition
- Generating visualizations

Output plots go to `plots/` at the repo root.

> Network issues? The Allegheny plot requires downloading external data. If it fails, the script continues without it.

---

## Common Issues

**Missing numpy?**
```bash
source .venv/bin/activate
pip install -r requirements.txt
```

**Julia not found?**
Install it from the official website or through your system's package manager.