# README: Ethical Allocation Simulation Framework

Welcome to the **Ethical Allocation Simulation Framework**! This framework enables researchers to explore and analyze various allocation strategies using different philosophical principles embedded in AI agents.

This repository contains code for the paper, "Ethics in Action: Comparative Analysis of Philosophical Frameworks in Resource Allocation using AI Agents".

---

## Features
- **Individual Allocator**: Distributes resources based on individual needs and fairness criteria.
- **Social Allocator**: Focuses on community-level distribution, considering socioeconomic and historical contexts.
- **Veil of Ignorance Allocator**: Allocates resources using the maximin principle to maximize welfare for the least advantaged.
- **Simulation Scenarios**: Includes static, dynamic, and cultural scenarios for comprehensive evaluation.

---

## Prerequisites
Ensure you have the following installed:
- Python 3.8+
- Conda (Anaconda or Miniconda)

---

## Setup
Create and activate the Conda environment:
   ```bash
   conda env create -f conda.yaml
   conda activate ethical-sim
   ```

---

## Running Simulations
1. Execute the experiments:
   ```bash
   python run_simulation.py
   ```

   - The simulation will generate results for various agents and scenarios.
   - Outputs include:
     - **Detailed JSON Results**: Stored in `simulation_results`.
     - **Summary CSV**: Includes metrics like equity, welfare, and Gini coefficient.

2. Adjust parameters:
   - Modify `run_simulation.py` to change the number of episodes, scenario types, or agents.
   - Example:
     ```python
     env = SimulationEnvironment(output_dir="custom_results", num_episodes=50)
     ```

---

## Results
### Output Files
- **Detailed Results**: JSON files in `simulation_results/`
- **Summary**: CSV files summarizing key metrics for comparison

### Key Metrics
- Minimum Welfare
- Average Welfare
- Equity Score
- Gini Coefficient

---

## Customization
### Add New Agents
1. Create a new agent class in the `agents` directory.
2. Implement the `process` and other relevant methods based on `BaseAgent`.
3. Include your agent in `run_simulation.py`.

### Add New Scenarios
1. Modify `scenarios.py` to define new scenario types.
2. Generate data relevant to your research objectives.

---

## Support
For questions or contributions, please open an issue or submit a pull request. Happy researching!
