Readme · MDCopyDrug–Drug Interaction Analysis Pipeline
# A Python pipeline that screens for potential drug–drug interactions (DDIs) using the DrugBank vocabulary. It standardizes drug-name data, matches free-text drug names to DrugBank entries (exact name → synonyms → partial match), detects pairwise interactions, and produces CSV reports and a network visualization to support clinical decision-making.

# Author: Mimi Adu-Serwaah, PharmD, MS
# Features

Standardize and clean DrugBank vocabulary data
Match free-text drug names to canonical DrugBank entries (exact, synonym, partial)
Detect pairwise drug–drug interactions
Generate CSV reports and a network-graph visualization
Produce a summary suitable for decision support

Tech stack
Python · pandas · networkx · matplotlib
Data (not included)
This repository does not redistribute DrugBank data. Download the DrugBank vocabulary CSV
from go.drugbank.com under its free academic license and place it at:

cd drug-interaction-pipeline
pip install -r requirements.txt
