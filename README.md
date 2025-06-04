# Energy-Efficient Building Design Recommendations using Deep Reinforcement Learning

This project leverages **Deep Reinforcement Learning (DRL)** techniques to recommend energy-efficient building designs. The goal is to minimize energy consumption by optimizing building parameters such as **window size**, **insulation thickness**, and **HVAC setpoint**.

## Project Overview

- **Environment**: A simulated building environment that models energy consumption based on design parameters.
- **Agent**: A Deep Q-Network (DQN) is used to learn optimal design strategies.
- **Goal**: Reduce energy consumption and provide actionable design recommendations for sustainable building development.

## Project Structure

```
📁 Energy-Efficient-Building-Design-DRL
├── building_env.py                   # Custom Gym environment for building simulation
├── dqn_agent.py                       # Deep Q-Network agent
├── train.py                            # Training loop
├── building_design_training_data.xlsx # Training log data
├── README.md                           # Project documentation
├── requirements.txt                    # Python dependencies
└── .gitignore                           # Ignored files and folders
```

## Requirements

Install all dependencies using:

```bash
pip install -r requirements.txt
```

**`requirements.txt` includes:**

```
torch
gym
numpy
pandas
openpyxl
```

## How to Run

1. Clone the repository and navigate into the project directory:

```bash
git clone https://github.com/your-username/Energy-Efficient-Building-Design-DRL.git
cd Energy-Efficient-Building-Design-DRL
```

2. Train the DRL agent:

```bash
python train.py
```

3. After training:
   - Evaluation metrics such as **energy consumption** and **rewards** will be printed.
   - Training logs will be saved to `building_design_training_data.xlsx`.

## Sample Environment Setup

Each building design consists of:
- **Window Size**: Continuous value between 0 and 1
- **Insulation Thickness**: Continuous value between 0 and 1
- **HVAC Setpoint**: Continuous value between 0 and 1

The DRL agent learns to recommend optimal settings to minimize the building's energy consumption.

## Dataset Example

```csv
Episode,Window_Size,Insulation_Thickness,HVAC_Setpoint,Energy_Consumption,Reward
1,0.3745,0.9507,0.7319,134.58,-72.36
2,0.5986,0.1560,0.1559,96.45,-88.21
...
```

## Output

- **`building_design_training_data.xlsx`**: Contains the design parameters, energy consumption, and reward for each episode.
- **Trained Model**: Saved as `building_design_dqn.pth`.

## Acknowledgements

- Inspired by energy-efficient building standards and sustainable design principles.
- Future work can integrate advanced simulation tools like **EnergyPlus** or **OpenStudio** for realistic energy modeling.

## Author

**Ayebawanaemi Geraldine Winston**

