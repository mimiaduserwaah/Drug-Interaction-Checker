python src/pipeline.py --drugs aspirin warfarin metformin

drug-interaction-pipeline/
│── README.md
│── requirements.txt
│── LICENSE
│── data/
│    └── chembl_35.db   ( do NOT commit large ChEMBL DB, add a note to download it)
│── notebooks/
│    └── demo_pipeline.ipynb   (My Jupyter Notebook with step-by-step analysis)
│── src/
│    └── pipeline.py           (clean modular Python script version)
│── outputs/
│    ├── example_network.png
│    ├── drug_mechanisms.csv
│    ├── drug_interactions.csv
│    ├── drug_atc.csv
│    └── drug_warnings.csv




# Drug-Interaction-Checker

# Drug–Drug Interaction Analysis Pipeline

This project implements a **modular pipeline** to analyze potential drug–drug interactions (DDIs) 
using the ChEMBL database (v35). It integrates **mechanism of action, target overlap, 
ATC classification, and clinical warnings** into a unified workflow.

##  Features
- Map free-text drug names to canonical ChEMBL identifiers
- Extract **mechanism of action** and biological targets
- Retrieve **ATC pharmacological classifications**
- Retrieve **clinical warnings** (e.g., black box warnings)
- Detect **pairwise drug–drug interactions** based on target overlap
- Generate **CSV reports** and a **network visualization**
- Produce a **summary report** for decision support

## Example Output
- Mechanisms: `drug_mechanisms.csv`
- ATC classes: `drug_atc.csv`
- Clinical warnings: `drug_warnings.csv`
- Interactions: `drug_interactions.csv`
- Visualization: `drug_network.png`

![Example Network](outputs/example_network.png)

## Installation
```bash
git clone https://github.com/mimiaduserwaah/drug-interaction-pipeline.git
cd drug-interaction-pipeline
pip install -r requirements.txt
