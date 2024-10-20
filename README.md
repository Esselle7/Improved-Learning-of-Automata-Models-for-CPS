# Improved Learning of Automata Models for Cyber-Physical Systems
## Overview

This repository contains the implementation of an enhanced approach for modeling Cyber-Physical Systems (CPS) by integrating the Sparse Identification of Nonlinear Dynamics (SINDy) method with the L*SHA algorithm. This integration enables dynamic behaviors to be modeled directly from observational data without relying on predefined Ordinary Differential Equations (ODEs).

## Contribution

This project builds upon the existing L*SHA framework. For details on the original L*SHA algorithm and its usage, please refer to the following repository:

[L*SHA Repository](https://github.com/LesLivia/lsha/tree/develop_pysindy)

### Key Features
- Integration of SINDy for improved CPS modeling.
- Ability to derive models directly from observational data.
- Flexible approach suitable for both known and unknown systems.

## Usage Instructions

1. **Clone the Repository**

   To get started, clone this repository to your local machine using the following command:

   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
2. **Install requirements**
  Ensure you have the necessary packages installed. You can do this using pip:
   ```bash
   pip install -r requirements.txt
3. **Run the L*SHA with pysindy**
  Follow readme_pysindy instructions and run the algorithm

## Executive Summary

This repository contains research and implementation files related to enhancing the modeling of Cyber-Physical Systems (CPS) through the integration of Sparse Identification of Nonlinear Dynamics (SINDy) with the L*SHA algorithm. CPS are increasingly important in various sectors, including manufacturing, transportation, healthcare, and energy, as they combine computational algorithms with physical processes. Accurate modeling and control of the often nonlinear and complex behaviors of CPS is a significant challenge addressed in this work.

### Objectives

The main goal of this research is to enhance CPS modeling by incorporating SINDy into the L*SHA framework, removing the reliance on predefined Ordinary Differential Equations (ODEs) and improving adaptability to unknown system dynamics. The PySINDy library is utilized to apply SINDy to real-world CPS data, allowing for autonomous refinement of models from observational data. Various case studies validate the proposed methodology, demonstrating its effectiveness in both well-understood and less-known systems.

### Key Concepts

- **Stochastic Hybrid Automata (SHA)**: Combines continuous and discrete dynamics, suitable for CPS modeling.
- **L*SHA Algorithm**: An enhanced learning framework that iteratively refines models based on environmental interactions and observed data.
- **Sparse Identification of Nonlinear Dynamics (SINDy)**: A method that discovers governing equations directly from data, enhancing the model discovery process.

### Model Training and Integration

The repository includes methods for training PySINDy models and integrating them into the L*SHA algorithm. Key steps include data preparation, model construction, optimization, and validation. Two training approaches are discussed:
- **Offline Method**: PySINDy models are trained prior to the learning process.
- **Online Method**: PySINDy is integrated directly into the identification phase between the teacher and learner.

### Verification Ready Model Generation

Models generated from the learned automata are adapted for verification tools like UPPAAL, ensuring they are suitable for rigorous evaluation against real-world scenarios.

### Case Studies

The methodologies were applied and validated across various case studies, including:

1. **Thermostat System**: A well-understood CPS where the relationship between operational states and temperature dynamics was effectively modeled.
2. **Human-Robot Interaction (HRI)**: Focused on estimating fatigue levels based on activity, with successful modeling of heart rate dynamics.
3. **Auto-twin Pizza Line**: A semi-known system modeling the pizza production process, predicting power dissipation with high accuracy.
4. **Energy MADE**: An unknown system where models were derived from data without prior knowledge of the governing dynamics.

### Future Improvements

Future work will explore the integration of advanced machine learning techniques, such as Artificial Neural Networks (ANNs) and Reinforcement Learning (RL), to further enhance model accuracy and reliability. These methods can help tackle challenges related to noisy data and complex system dynamics.

## Repository Contents

- **Colab Notebooks**: Implementation of the methodologies discussed in the research.
- **PDF of Executive Summary**: A comprehensive overview of the research findings.

## Requirements

To run the Colab notebooks, ensure you have the following libraries installed:
- PySINDy
- NumPy
- Matplotlib
- [Other dependencies as needed]

## Usage

1. Open the Colab notebooks provided in this repository.
2. Follow the instructions within each notebook to replicate the experiments and explore the methodologies.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

Special thanks to the contributors and researchers who provided insights and data for the case studies.

