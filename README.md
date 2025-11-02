🔬 Quantum Kernel Methods for Cancer Diagnosis: A Bio-Inspired Approach
This project demonstrates the application of Quantum Support Vector Classification (QSVC) to a binary medical diagnosis task, specifically classifying breast tumors (Benign vs. Malignant) based on cellular features.

Key Highlights:

Feature Engineering with Inductive Bias: The 10 original input features were systematically grouped into 5 biologically meaningful factors (Size, Shape, Irregularity, Texture, Global Geometry) to introduce domain knowledge (an "inductive bias") into the quantum model. This step reduced the required quantum circuit size to 5 qubits.

Feature Map Comparison: We compared two distinct 5-qubit Quantum Feature Maps for encoding the data:

Standard ZZ Feature Map: A generic map with full entanglement between all qubits, serving as a baseline.

Custom Bio-Inspired Feature Map: A novel map with selective entanglement designed to explicitly connect the biologically related factors (e.g., Size ↔ Shape).

Performance Result: The QSVC model utilizing the Custom Bio-Inspired Feature Map (88.8% accuracy) significantly outperformed the model based on the Standard ZZ Map (75.5% accuracy) on the test set.

Conclusion: The results validate that incorporating domain-specific knowledge directly into the quantum circuit's structure is critical for enhancing performance in quantum machine learning applications.

Technologies Used:

Qiskit / Qiskit-Machine-Learning

NumPy and Pandas for data handling

Scikit-learn for data preprocessing and final SVM training
