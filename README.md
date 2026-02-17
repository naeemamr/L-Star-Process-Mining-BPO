# Process Mining Implementation: Recreating the L* Methodology

This project recreates the process mining **L* life cycle methodology** as detailed in the research paper *"Applying Process Mining: The Reality of a Software Development SME"*. [cite_start]The implementation uses a custom BPO dataset to demonstrate the portability of the framework beyond its original application.

## 📑 Project Overview
[cite_start]The goal of this project is to apply advanced process mining techniques—Discovery and Conformance Checking—to understand and optimize business processes.

### The L* Life Cycle Stages
The project follows the four-stage L* methodology outlined in the paper:
1. [cite_start]**Stage 1: Plan and Extract** – Pre-processing raw data to create an event log (Case ID, Activity, Timestamp).
2. [cite_start]**Stage 2: Discovery** – Generating a process model (Petri net/BPMN) using the **Inductive Miner** algorithm[cite: 1].
3. [cite_start]**Stage 3: Conformance** – Using **Token-Based Replay (TBR)** to measure how well the discovered model fits the actual event log[cite: 1].
4. [cite_start]**Stage 4: Enhancement** – Identifying bottlenecks and suggesting process improvements.

## 🛠️ Technical Stack
- **Language:** Python
- **Libraries:** PM4Py, Pandas, Matplotlib
- **Tooling:** Jupyter Notebook

## 📂 Repository Structure
- [cite_start]`Process Mining.ipynb`: The main implementation notebook containing data cleaning, discovery, and conformance code[cite: 1].
- [cite_start]`applsci-14-01402.pdf`: The foundational research paper by Urrea-Contreras et al.[cite: 2].
- `datasets/`: Contains the three BPO datasets used for the analysis.

## 🚀 How to Run
1. Clone the repository.
2. Install dependencies: `pip install pm4py pandas matplotlib`.
3. [cite_start]Open `Process Mining.ipynb` and run the cells to view the generated Petri nets and fitness scores[cite: 1].

## 📊 Results
[cite_start]The implementation successfully calculated fitness scores via Token-Based Replay, identifying specific deviations between the planned process and the actual execution recorded in the BPO logs[cite: 1].
