
Project Overview

This repository contains the Python code and associated resources for the final project report titled "A Simulation Model on Coil Production System for Inventory and Capacity Analysis Through Optimization Process" (ENG5814: Industry-Based Project B: Monash University Malaysia). The project, authored by Maisha Mashiata (Monash Student ID: 35431180) under the supervision of Dr. Ts. Ho Kok Hoe, develops a simulation-based framework to optimize inventory management and production capacity in BlueScope's coil production system. The simulation replicates the multi-stage coil manufacturing process (slitting, cleaning, thickness reduction, quality control, and delivery) observed during an industrial visit to BlueScope on October 3, 2024. Using Visual Components for 3D simulation and Python for data analysis and optimization, the project addresses operational challenges such as inventory imbalances, capacity constraints, and bottlenecks.

Features

Simulation Model: Built using Visual Components to replicate BlueScope's coil production process, including slitting, cleaning, thickness reduction, quality control, and delivery stages.
Inventory and Capacity Analysis: Analyzes inventory levels and throughput using metrics like average inventory, maximum inventory, and throughput per conveyor.
Lean (Muda) Analysis: Identifies inventory, waiting, and overproduction waste to highlight inefficiencies.
Bottleneck Analysis: Computes bottleneck scores to pinpoint congestion points, particularly at the thickness reduction stage (Conveyor #7).
Hybrid Optimization: Implements a hybrid Differential Evolution (DE) and Sequential Least Squares Programming (SLSQP) approach to optimize processing times, achieving a 25% throughput efficiency gain.
Visualization: Generates time-series plots, bar charts, heatmaps, pie charts, and scatter plots to visualize inventory, throughput, waste, and bottleneck metrics.


Prerequisites

Python: Version 3.8 or higher


Required libraries include:
pandas for data manipulation
numpy for numerical computations
matplotlib and seaborn for visualization
scipy for optimization (DE and SLSQP)


Usage

Run Analysis:Execute the main analysis script to process simulation data and generate metrics for inventory, capacity, lean waste, and bottlenecks

This script reads CSV files from data and outputs metrics to the console and saves visualizations

Run Optimization:Execute the optimization script to apply the hybrid DE-SLSQP approach, adjusting processing times to minimize bottlenecks while maintaining throughput:

Outputs optimized processing times, inventory levels, and throughput metrics to the console 

Generate Visualizations:Run the visualization script to create plots (e.g., time-series, heatmaps, pie charts)



Data

Input Files:
conveyor_metrics.csv: Contains metrics like coils entered, current, and exited per conveyor.
time_metrics.csv: Contains processing times (minimum, maximum, total) per conveyor.


Output Files:
Visualization figures (e.g., inventory_over_time.png, throughput_heatmap.png) 
Analysis results printed to the console 



Key Findings

Inventory Analysis: Significant stock accumulation at Conveyor #7 (max 15 coils), indicating overstocking risks at the thickness reduction stage.
Capacity Analysis: Low throughput at Conveyor #7 (0.01 coils/time), confirming it as a critical bottleneck.
Lean Analysis: Waiting waste dominates (1900 units), driven by delays at Conveyor #7.
Bottleneck Analysis: Conveyor #7 contributes 67.4% to the total bottleneck score (8000 units).
Optimization: Achieved a 25% throughput efficiency gain, reducing Conveyor #7's processing time from 1196.50 to 957.20 units and inventory from 6.5 to 5.45 units.

Future Work

Implement real-time adaptive optimization using reinforcement learning.
Incorporate sustainability metrics (e.g., energy consumption, material waste).
Extend the model to include supply chain dynamics (e.g., supplier scheduling).
Explore digital twin technologies for real-time monitoring.
Validate the model across different coil production facilities or material types.

Acknowledgments

Supervisor: Dr. Ts. Ho Kok Hoe for guidance and support.

BlueScope: For providing access to their coil production facility on October 3, 2024.

Tools: Visual Components for simulation, Python libraries (Pandas, NumPy, Matplotlib, Seaborn, SciPy) for analysis and optimization.


For questions or contributions, please contact:

Author: Maisha Mashiata (Monash Student ID: 35431180)
Email: [mmas0049@student.monash.edu]/Email: [mashiatamaisha@gmail.com]

