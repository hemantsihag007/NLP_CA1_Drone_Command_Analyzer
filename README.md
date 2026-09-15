# Smart Drone Command Language Analyzer Using Basic NLP

Natural Language Processing (CSE 306) — CA Project

## Overview
A basic rule-based NLP application that analyzes simple delivery-drone commands.

## Features
- Tokenization
- Subject / Verb / Object identification
- Simple parsing
- Corpus-based sentence validation
- Rejection reasons
- Dynamic corpus addition
- Corpus display
- Vocabulary display
- Interactive menu
- Test cases and result visualization

## Dataset
Initial corpus: 20 custom sentences.

Subjects: `drone`, `robot`

Verbs: `carries`, `delivers`, `drops`, `moves`, `picks`, `transports`

Objects: `box`, `food`, `goods`, `medicine`, `package`, `parcel`

## Example
`Drone delivers package`

Output:
- Subject → drone
- Verb → delivers
- Object → package
- Status → Accepted

## Files
- `NLP_CA1_Drone_Command_Analyzer.ipynb` — main Jupyter Notebook
- `Drone_Command_NLP_Project_Report.docx` — short report
- `Drone_Command_NLP_Project_Report.pdf` — PDF report
- `Drone_Command_NLP_Project_Presentation.pptx` — presentation

## Submission
Deploy the notebook on ByteXL Nimbus and submit the GitHub repository link as required by the CA instructions.
