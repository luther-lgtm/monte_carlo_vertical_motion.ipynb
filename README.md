# Monte Carlo Simulation of Vertical Motion Under Uncertainty

🔗 **[Original model built in Google Sheets ](https://docs.google.com/spreadsheets/d/1uag_EHIpRTyykQFWzIN6hjBPhMk0EXLU7_RQN3mNygo/edit?usp=sharing)**

🔗 **[Run the simulation in Google Colab ](https://colab.research.google.com/drive/12u_qRsGwf-Q0_YUudEXgws8Nn-L8Y8w3)**

🔗 **[View the GitHub repository](https://github.com/luther-lgtm/monte_carlo_vertical_motion.ipynb/tree/main)**




## Overview
This project uses a Monte Carlo simulation to model one-dimensional vertical motion and examine how randomness in initial velocity affects trajectory and maximum height. The model combines classical kinematics with probabilistic sampling to study uncertainty propagation in a physical system.

The simulation is implemented using data from Google Sheets and analyzed in a browser-based Jupyter notebook (Google Colab), making it fully reproducible on a Chromebook.

## Motivation
Introductory physics problems typically assume exact initial conditions. In practice, measurements and launch conditions vary. This project explores how small variations in initial velocity translate into variance in physical outcomes, using Monte Carlo methods to move beyond deterministic assumptions.

## Data
Initial velocity values are sourced from a Google Sheets dataset and used to estimate:
- Mean initial velocity
- Standard deviation of initial velocity

These empirical parameters define the probability distribution used in the simulation.

## Methodology
- Sample initial velocities from a normal distribution
- Simulate vertical motion under constant gravitational acceleration
- Compute position–time trajectories for many trials
- Record maximum height for each trial
- Analyze variance and distribution of outcomes

Ground contact is enforced for visualization by constraining height to non-negative values.

## Energy Analysis
With faculty supervision, the model was extended to compute:
- Kinetic energy
- Gravitational potential energy
- Total mechanical energy

Energy is evaluated only while the projectile remains above ground to avoid post-impact artifacts. This verifies conservation of energy across Monte Carlo trials despite uncertainty in initial conditions.

## Key Insights
- Small variations in initial velocity produce measurable variance in maximum height
- Uncertainty propagates predictably through deterministic equations of motion
- Total mechanical energy remains conserved prior to ground contact
- Monte Carlo methods provide a natural framework for studying physical systems with uncertain inputs

## Tools
- Google Sheets (data source)
- Python (NumPy, Pandas, Matplotlib)
- Google Colab (Chromebook-compatible execution)

## Files
- `monte_carlo_vertical_motion.ipynb` — simulation and analysis notebook

## Author
Independent undergraduate project focused on uncertainty propagation, classical mechanics, and probabilistic modeling.
