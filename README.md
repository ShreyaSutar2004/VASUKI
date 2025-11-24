VASUKI – From Myth to Molecule 

VASUKI is an integrated, GUI-based automation tool designed to simplify the entire homology modeling workflow using Modeller, BLAST, and Python. The tool eliminates the need for manual command-line operations and provides a clean, interactive interface for researchers, students, and computational biologists.

📌 Overview

Homology modeling is a powerful method for predicting 3D protein structures when experimental structural data isn’t available. However, running Modeller manually involves multiple steps:

Running BLAST

Selecting the best templates

Performing sequence alignment

Preparing .ali and .py model files

Running Modeller scripts

Evaluating and visualizing the models

These steps are time-consuming and prone to error.

VASUKI automates this entire pipeline with a user-friendly graphical interface.

  Key Features
  
🔍 1. Integrated BLAST Search Panel

Paste or upload a FASTA sequence

Run BLAST locally or through NCBI

Automatically extract best template PDB IDs

Option to download template structures

🧬 2. Smart Template–Target Alignment

Uses Modeller's Alignment() for multiple sequene alignment

Generates PIR files automatically

Highlights identity & similarity

🏗️ 3. Automated Model Building (Modeller Engine)

Uses Modeller’s:

Environment()

AutoModel()

Alignment()

Builds multiple models

Stores all logs, DOPE scores, and PDBs

🤖 4. Modssitant AI Assistant Integration

Powered by HuggingFace and LangChain

Provides intelligent suggestions and automated guidance through the modeling workflow

Chatbot interface for user queries and troubleshooting

Helps with interpreting results and next steps

📊 5. Quality Assessment & Evaluation

Extracts DOPE, molpdf, GA341

Identifies the best-scoring model

Prepares a mini-report inside the output folder

🖥️ 6. Clean, Modern, Draggable GUI

Built using PyQt5

Uses QSplitter-based adjustable panels

Full console logging

Error checking & messaging

Lightweight & modular

🧪 7. External Visualization Support

Integrated in the software, cartoon structure

using 3Dmol.js and PyQt5WebEngine

Shows model list & output directory

Tech Stack Used
Languages & Frameworks

Python 3.10+

PyQt5 (GUI)

Modeller (core homology modeling)

Biopython (BLAST, parsing, alignment)

AI / Language Models

HuggingFace Transformers — hosting LLM models

LangChain — chaining prompts and handling conversational flow for Modssitant AI assistant

Additional Libraries

subprocess

requests

pathlib

os

Bio.Align, Bio.SearchIO

⚙️ Installation & Setup

1️⃣ Clone the Repository
git clone https://github.com/ShreyaSutar2004/VASUKI.git
cd VASUKI 

2️⃣ Create and Activate a Virtual Environment
python -m venv .venv
.venv\Scripts\activate       # Windows

3️⃣ Install Dependencies
 Create a simple requirements.txt file : 
 PyQt5>=5.15.4
modeller
biopython
requests
langchain
transformers
PyQt5WebEngine

pip install -r requirements.txt

4️⃣ Install Modeller

Obtain a license key from:
https://salilab.org/modeller/

Then:

pip install modeller

Add to PATH.

6️⃣ Run VASUKI 
python main.py

Future Enhancements for VASUKI 

DOPE profile plotting

Ramachandran plot generator

Mutation analysis module

Improved model refinement

MD simulation setup

Full ecosystem:
Homology Modeling → Refinement → MD → Post-analysis → Reports

Integration with AI/LLM-based assistants for model selection

GUI-based template editor




