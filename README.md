# QNova-Quantum-Hackathon
QNova – AI-powered quantum computing project for optimization and intelligent problem-solving.
 Q-WATER — Quantum-Assisted Irrigation Water Allocation

 Project Overview

Q-WATER is a quantum optimization prototype designed to explore how limited irrigation water can be allocated among different crops. It combines classical optimization with quantum computing techniques to compare water-allocation decisions under a fixed water budget.

The project uses a QUBO (Quadratic Unconstrained Binary Optimization) model and the Quantum Approximate Optimization Algorithm (QAOA) through Qiskit.

 Problem Statement

Water is a limited agricultural resource. Farmers need to distribute available irrigation water among crops while considering each crop's water requirements and priority.

Q-WATER models this problem as an optimization task with a total water limit of 10,000 litres.

✨ Key Features

- Crop-wise irrigation water allocation
- Classical baseline for comparison
- QUBO-based optimization model
- QAOA simulation using Qiskit
- Classical-versus-quantum result comparison
- Allocation table and bar chart
- Dashboard-style results summary

🌾 Crops and Water Allocation

The prototype considers four crops:

Crop| Water Requirement| Classical Allocation| QAOA Allocation
Rice| 4,000 L| 4,000 L| 3,000 L
Tomato| 2,000 L| 2,000 L| 2,000 L
Maize| 3,000 L| 3,000 L| 3,000 L
Groundnut| 2,500 L| 1,000 L| 2,000 L
Total| —| 10,000 L| 10,000 L

⚙️ Technologies Used

- Python
- Google Colab
- Qiskit
- Qiskit Optimization
- Qiskit Aer
- Pandas
- Matplotlib
- QUBO optimization
- QAOA simulation

🧠 How It Works
flowchart TD
    A["Crop Data and Water Budget"] --> B["Python Data Processing"]
    B --> C["Classical Optimization Baseline"]
    B --> D["QUBO Model Formulation"]
    D --> E["QAOA Algorithm"]
    E --> F["Qiskit Simulator"]
    C --> G["Compare Results"]
    F --> G
    G --> H["Allocation Table"]
    G --> I["Comparison Bar Chart"]
    H --> J["Q-WATER Dashboard"]
    I --> J

  SYSTEM FLOWCHART
  flowchart TD
    A["Crop Data and Water Budget"] --> B["Python Data Processing"]
    B --> C["Classical Optimization Baseline"]
    B --> D["QUBO Model Formulation"]
    D --> E["QAOA Algorithm"]
    E --> F["Qiskit Simulator"]
    C --> G["Compare Results"]
    F --> G
    G --> H["Allocation Table"]
    G --> I["Comparison Bar Chart"]
    H --> J["Q-WATER Dashboard"]
    I --> J
  

1. Input data: Define the crops, water requirements, priorities, and available water.
2. Classical baseline: Calculate a conventional allocation for comparison.
3. QUBO formulation: Represent the allocation problem as a binary optimization model.
4. Quantum optimization: Run QAOA using a quantum-circuit simulator.
5. Comparison: Compare the classical and QAOA allocations and objective scores.
6. Visualization: Display the results in a table, graph, and dashboard-style summary.

📊 Results

Method| Objective Score| Total Water Allocated
Classical baseline| 13.20| 10,000 L
QAOA simulator| 13.15| 10,000 L

Both solutions satisfy the model's 10,000-litre water limit. In this experiment, the classical baseline achieved a slightly higher objective score than the QAOA result.

Important finding: This prototype demonstrates the application of QUBO and QAOA to irrigation allocation. The current results do not demonstrate quantum advantage; further testing and benchmarking are required.

🚀 How to Run

1. Open Google Colab.
2. Upload or open the project's ".ipynb" notebook.
3. Run the notebook cells in order.
4. Review the classical allocation and QAOA simulation results.
5. View the comparison graph and dashboard output.

🌍 Potential Applications

- Agricultural water-resource planning
- Crop-priority-based irrigation allocation
- Optimization under limited resources
- Educational demonstrations of quantum optimization
- Research into hybrid classical–quantum approaches

🔮 Future Improvements

- Test additional crop combinations and water budgets.
- Compare QAOA across different circuit depths and optimizer settings.
- Benchmark against more classical optimization methods.
- Explore execution on real quantum hardware.
- Improve the dashboard and investigate real-world agricultural data.
- Evaluate solution quality and runtime across larger problem instances.

👥 Project Status

Status: Hackathon prototype

Q-WATER is an experimental proof of concept. Its results are based on the current model and simulator configuration and should not yet be treated as validated agricultural recommendations.

📜 License

Choose a suitable open-source license before distributing the project publicly. For example, you may use the MIT License if it fits your team's requirements.
