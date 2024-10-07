
# Topsis Package

Python Package for TOPSIS Analysis in Multi-Criteria Decision Making


## Authors

- [@Guryansh](https://www.github.com/Guryansh)


## Features

- Customizable Decision Matrix
- Comprehensive Error Handling


## Installation

Install the package with following command

```bash
  pip install Topsis-Guryansh-102218044
```
    
## Usage
- Weights and Imapcts seperated by commas
- Impacts should be give in + and - for maximization and minimization respectively
- Files should be of format .csv
- If anu input contains spaces, make sure to enclose it between double quotes (" ").
```bash
guryansh_topsis <inputFileName> <Weights> <Impacts> <resultFileName>
```

## Example

### Sample Input File Format
The input CSV file should have the following structure:

| Fund Name | P1  | P2  | P3  | P4  | P5  |
|-----------|-----|-----|-----|-----|-----|
| M1        | 0.84| 0.71| 6.7 | 42.1| 12.59|
| M2        | 0.91| 0.83| 7.0 | 31.7| 10.11|
| ...       | ... | ... | ... | ... | ... |

- weights vector = [ 0.25 , 0.25 , 0.25 , 0.25 , 0.25 ]
- impacts vector = [ - , + , + , + , + ]

```javascript
guryansh_topsis 102218044-data.csv ".25,.25,.25,.25,.25" "-,+,+,+,+" output.csv

```

### Sample Output File Format

The output CSV file will have the following structure:

| Fund Name | P1  | P2  | P3  | P4  | P5  | Topsis Score | Rank |
|-----------|-----|-----|-----|-----|-----|--------------|------|
| M1        | 0.84| 0.71| 6.7 | 42.1| 12.59| 0.3653       | 6    |
| M2        | 0.91| 0.83| 7.0 | 31.7| 10.11| 0.2819       | 8    |
| ...       | ... | ... | ... | ... | ...  | ...          | ...  |


[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
