

Qiskit Fall Fest 2026 — Quantum Computing Challenges
A collection of Jupyter Notebook solutions developed as part of Qiskit Fall Fest 2026, organized by IBM Quantum in collaboration with Vishnu Institute of Technology.

This repository contains quantum computing experiments implemented using Qiskit, with circuit visualizations, simulations, measurement results, and histograms.

📂 Repository Contents
File	Description
Challenge 1.ipynb	Jupyter Notebook solution for Challenge 1
Challenge 2.ipynb	Jupyter Notebook solution for Challenge 2
Challenge 3.ipynb	Investigating how a quantum gate changes the correlation between two qubits
Challenge 4.ipynb	Switching between correlated and opposite measurement outcomes
🎯 Objectives
Learn the fundamentals of quantum circuits using Qiskit.

Create and execute quantum circuits with two qubits.

Understand quantum gates and their effects on measurement outcomes.

Simulate quantum experiments and analyze measurement counts.

Visualize and compare experimental results using histograms.

Explore correlations and entanglement in two-qubit systems.

🛠️ Technologies Used
Python

Qiskit — Quantum circuit creation and simulation

Qiskit Aer — Quantum circuit simulator

Matplotlib — Data visualization and histograms

NumPy — Numerical operations

Jupyter Notebook / Google Colab — Interactive development environment

🚀 Getting Started
Option 1: Google Colab
Open the notebook you want to execute.

Upload it to Google Colab.

Install the required libraries in a code cell:

%pip install qiskit qiskit-aer matplotlib numpy
Run the notebook cells in order.

Observe the quantum circuits, measurement counts, and histograms.

Option 2: Run Locally
Install Python and Jupyter Notebook, then install the dependencies:

pip install qiskit qiskit-aer matplotlib numpy notebook
Clone this repository:

git clone https://github.com/Vinay32592/Qiskit-Challenges.git
Navigate to the repository directory:

cd Qiskit-Challenges
Launch Jupyter Notebook:

jupyter notebook
Open any challenge notebook and execute the cells in order.

🔬 Challenge Highlights
Challenge 3 — Can You Change the Correlation?
Investigates how modifying a Bell-state circuit with an additional quantum gate changes the relationship between two-qubit measurement outcomes.

Challenge 4 — Quantum Correlation Switch
Demonstrates two different measurement behaviors:

Correlated outcomes: 00 and 11

Opposite outcomes: 01 and 10

The circuits are simulated for 100 shots each, and the measurement results are compared using histograms.

📊 Results and Visualization
The notebooks demonstrate quantum circuit structures, measurement counts, and graphical comparisons of possible measurement outcomes.

For the ideal simulated circuits in Challenges 3 and 4, the expected outcomes illustrate how quantum gates can change the measurement relationship between qubits.

📚 Learning Outcomes
Understanding quantum circuit construction.

Applying Hadamard, CNOT, and Pauli-X gates.

Exploring Bell states and two-qubit correlations.

Executing circuits with a quantum simulator.

Analyzing measurement results and visualizing data.

👨‍💻 Author
Vinay32592

GitHub: @Vinay32592

Acknowledgment
Developed as part of the Qiskit Fall Fest 2026 learning activities associated with IBM Quantum and Vishnu Institute of Technology.

Exploring quantum computing one circuit at a time.


