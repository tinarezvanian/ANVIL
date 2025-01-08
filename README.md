# ANVIL: AI-Driven eNgine for Vulnerability Identification Using LLMs

**Welcome to ANVIL**, an open-source project showcasing a proof-of-concept Large Language Model (LLM) that detects software vulnerabilities and generates proof-of-concept exploits. Our focus is on **automating vulnerability identification** in complex codebases, particularly those relevant to DoD aviation and missile systems.

---
## Highlights

- **Perfect Juliet Test Suite Score**  
  We achieved an F1 score of **1.0** on the publicly available [Juliet test suite](https://samate.nist.gov/SRD/testsuite.php) for classic C/C++ vulnerabilities.  
- **LoRA-Based Fine-Tuning**  
  Our approach uses [LoRA](https://arxiv.org/abs/2106.09685) (Low-Rank Adapters) to quickly and efficiently fine-tune an existing LLM (e.g., Code Llama) without retraining from scratch.
- **Code + Exploit Generation**  
  We provide proof-of-concept code demonstrating how to extend vulnerability detection to **exploit generation** workflows.
- **Tool/Agent Extensions**  
  Future work includes multi-step, tool-using LLMs for richer scanning, dynamic testing, and iterative exploit development.

---
## Repository Structure

- `vul_llm.ipynb`  
  A Jupyter notebook illustrating the end-to-end training process on the Juliet dataset.
- `scripts/`  
  Helper scripts for data preprocessing, tokenization, and model loading.
- `models/`  
  Contains configuration files and LoRA adapter checkpoints (if you wish to share or store them here).
- `data/`  
  Placeholder directory for any sample or preprocessed code data. (Juliet data not included by default due to licensing/distribution constraints.)

---
## Quick Start

1. **Clone the repo**  
   ```bash
   git clone https://github.com/tinarezvanian/ANVIL.git
   cd ANVIL
