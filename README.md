# Cheminformatics_Learning

# My Python & Cheminformatics Learning Journey

## About This Repository
I am an MSc student in Pharmacochemical and Pharmacological Development of Drug Molecules with a strong wet-lab background in Chemistry and Natural Products. I am currently expanding my skill set by learning Python from scratch to learn more about the field of Computational Drug Discovery.

This repository tracks my progress as I learn to code. 

## Script 01: The Basic Lipinski Weight Checker
**Concepts Learned:** 
*   Variables and Strings
*   Basic RDKit functions (`MolFromSmiles`, `Descriptors.MolWt`)
*   Conditional Logic (`if/else` statements)

**What the script does:** 
It takes a SMILES string of a molecule, calculates its molecular weight, and uses an `if/else` statement to automatically decide if it passes Lipinski's Rule of 5 for molecular weight (< 500 Da).


## Script 02: Dual-Parameter Lipinski Evaluation (MW & LogP)
**Concepts Learned:** 
* Extracting multiple chemical properties (`Descriptors.MolLogP`)
* Complex Conditional Logic (`if ... and ...`)
* Formatted Strings (f-strings) for cleaner data reporting

**What the script does:** 
It evaluates a natural bioactive molecule (e.g., Quercetin) against two crucial pharmacokinetic parameters simultaneously: Molecular Weight (< 500 Da) and Lipophilicity (LogP < 5). It outputs a structured report concluding whether the compound meets the combined drug-like criteria.


# Script 03: Full Lipinski Rule of 5 High-Throughput Screener
**Concepts Learned:** 
* Python Dictionaries and `for` loops for automation
* Calculating all 4 Lipinski parameters (MW, LogP, H-Donors, H-Acceptors)
* Using Counters (`+= 1`) to track rule violations
* Debugging common Python syntax errors

**What the script does:** 
It simulates a mini High-Throughput Screening (HTS) pipeline. It iterates through a library of compounds (including natural products like Quercetin and complex antibiotics like Erythromycin), calculates all four Lipinski descriptors, counts the number of violations, and strictly applies the pharmaceutical rule that a drug-like molecule must have $\le$ 1 violation.


## Script 04: Data Structuring and CSV Export with Pandas
**(Folder: 04_Pandas_Reporter)**

**Concepts Learned:** 
* Storing iteration results into a List of Dictionaries
* Utilizing the `pandas` library to create DataFrames
* Exporting computational data to `.csv` files for downstream analysis
* Project organization (keeping scripts and output data in dedicated directories)

**What the script does:** 
It upgrades the previous HTS screener by replacing raw text output with a structured `pandas.DataFrame`. After evaluating the compound library against Lipinski's rules, it automatically generates and exports a clean `lipinski_report.csv` file, demonstrating how cheminformatics pipelines prepare data for experimental scientists.
