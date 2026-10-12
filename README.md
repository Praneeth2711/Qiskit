# Qiskit Quantum Computing Challenges

Hands-on quantum circuit experiments built with Qiskit and Qiskit Aer.

[![GitHub](https://img.shields.io/badge/GitHub-View%20Notebooks-181717?logo=github)](https://github.com/Praneeth2711/Qiskit) [![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?logo=python&logoColor=white)](https://www.python.org/) [![Qiskit](https://img.shields.io/badge/Qiskit-Quantum%20circuits-6929C4)](https://www.ibm.com/quantum/qiskit)

Explore how quantum gates affect measurement, from a single qubit to correlated two-qubit Bell states. Each challenge is a Jupyter notebook with circuit diagrams, Aer simulation, measurement counts, and plots.

> These notebooks use a local ideal simulator. No IBM Quantum account or quantum hardware access is required.

## Challenges

| Notebook                           | Topic                  | What you will explore                                                                 |
| ---------------------------------- | ---------------------- | ------------------------------------------------------------------------------------- |
| [Challenge 1](Challenge%201.ipynb) | Predict the output     | Compare one `X` gate, two `X` gates, and an `H` gate on a single qubit.               |
| [Challenge 2](Challenge%202.ipynb) | Biased quantum coin    | Use `RY` rotations to favor measuring `0` or `1`, then compare the sampled counts.    |
| [Challenge 3](Challenge%203.ipynb) | Change the correlation | Create a Bell state, apply `X` to one qubit, and compare the possible joint outcomes. |
| [Challenge 4](Challenge%204.ipynb) | Correlation switch     | Build circuits that produce correlated versus opposite measurement outcomes.          |

## Expected Outcomes

These are ideal probabilities; finite-shot results can vary between runs.

| Challenge | Circuit                                          | Ideal measurement behavior            |
| --------- | ------------------------------------------------ | ------------------------------------- |
| 1         | One `X` gate                                     | `1` with probability 100%             |
| 1         | Two `X` gates                                    | `0` with probability 100%             |
| 1         | One `H` gate                                     | `0` and `1` with probability 50% each |
| 2         | `RY(pi/3)`                                       | `0` about 75%, `1` about 25%          |
| 2         | `RY(2*pi/3)`                                     | `0` about 25%, `1` about 75%          |
| 3-4       | Bell circuit: `H` then `CNOT`                    | Correlated outcomes: `00` or `11`     |
| 3-4       | Bell circuit followed by `X` on the second qubit | Opposite outcomes: `01` or `10`       |

Each notebook samples 100 shots per circuit and visualizes the returned counts. The `H` and `RY` circuits produce probabilistic results, so observed percentages will not always exactly match their ideal probabilities.

## Run Locally

You need Python 3.10 or later. From a terminal:

```bash
git clone https://github.com/Praneeth2711/Qiskit.git
cd Qiskit
python -m venv .venv
```

Activate the environment, then install the libraries.

```powershell
# Windows PowerShell
.venv\Scripts\Activate.ps1
python -m pip install qiskit qiskit-aer matplotlib numpy pandas notebook
```

```bash
# macOS / Linux
source .venv/bin/activate
python -m pip install qiskit qiskit-aer matplotlib numpy pandas notebook
```

Start Jupyter and open a challenge notebook:

```bash
jupyter notebook
```

Run the cells from top to bottom. The notebooks run circuits using `AerSimulator`.

## Run in Google Colab

1. Open a challenge notebook on GitHub.
2. Download it and upload the `.ipynb` file to [Google Colab](https://colab.research.google.com/).
3. Run the notebook cells from top to bottom. If prompted for dependencies, run `%pip install qiskit qiskit-aer matplotlib numpy pandas` in a code cell.

## Tools and Concepts

- **Qiskit:** quantum circuit construction, gates, and measurement
- **Qiskit Aer:** local circuit simulation
- **Matplotlib:** measurement histograms and comparisons
- **NumPy and pandas:** rotation parameters and tabular results
- **Jupyter Notebook:** interactive code and visualizations

The challenges introduce the Pauli-`X`, Hadamard, and `RY` gates; computational-basis measurement; Bell-state preparation with `CNOT`; shot sampling; and two-qubit correlations.

## About

Prepared for Qiskit Fall Fest 2026 challenge activities associated with IBM Quantum and Vishnu Institute of Technology.

**Author:** [Praneeth2711](https://github.com/Praneeth2711)
