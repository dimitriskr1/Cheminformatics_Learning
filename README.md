# Cheminformatics_Learning

# My Python & Cheminformatics Learning Journey

## About This Repository
I am an MSc student in Pharmaceutical and Pharmacological Development with a strong wet-lab background in Chemistry and Natural Products. I am currently expanding my skill set by learning Python from scratch to learn more about the field of Computational Drug Discovery.

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
