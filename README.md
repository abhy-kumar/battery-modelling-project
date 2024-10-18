# Battery Modeling Project

## Overview
This project implements various battery models to simulate and analyze battery behavior under different conditions. It includes implementations of State of Charge (SoC) and State of Health (SoH) calculations, as well as first-order and second-order RC (Resistor-Capacitor) equivalent circuit models.

## Table of Contents
1. [Dependencies](#dependencies)
2. [File Structure](#file-structure)
3. [Models Implemented](#models-implemented)
4. [Usage](#usage)
5. [Key Functions](#key-functions)
6. [Results](#results)
7. [Contributing](#contributing)

## Dependencies
- Python 3.x
- NumPy
- SciPy
- Matplotlib

## File Structure
The project consists of a single Python script containing all the implementations and visualizations.

## Models Implemented

### 1. State of Charge (SoC) and State of Health (SoH) Model
This model simulates battery aging and calculates the State of Charge over multiple cycles, considering factors such as:
- Calendar aging
- Cycle aging
- Depth of Discharge (DoD)
- Temperature effects

### 2. RC Equivalent Circuit Models
#### a. Basic RC Model
A simple implementation of the RC equivalent circuit model for batteries.

#### b. First-Order RC Model
An improved model that fits experimental data to a first-order RC equivalent circuit.

#### c. Second-Order RC Model
A more complex model that fits experimental data to a second-order RC equivalent circuit for increased accuracy.

## Usage
To run the simulations and generate plots:

1. Ensure all dependencies are installed.
2. Run the Python script.
3. The script will output various plots and parameter values for different models.

## Key Functions

### `rc_model(t, R1, C1, R0, I, V_oc)`
Implements the basic RC model equation.

### `second_order_rc_model(t, R1, C1, R2, C2, V_oc)`
Implements the second-order RC model equation.

### `curve_fit` from SciPy
Used to fit the experimental data to the RC models.

## Results
The script generates several plots:
1. RC Equivalent Circuit Model voltage response
2. Fitted First-Order RC Model vs. Experimental Data
3. Fitted Second-Order RC Model vs. Experimental Data
4. Residuals for both First-Order and Second-Order RC Models

Parameter values for the fitted models are printed to the console.

## Contributing
Contributions to improve the models or add new features are welcome. Please follow these steps:
1. Fork the repository
2. Create a new branch for your feature
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request

---

For any questions or issues, please open an issue in the project repository.
