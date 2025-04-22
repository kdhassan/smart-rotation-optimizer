# Fatigue-Aware Job Rotation Scheduler

An intelligent scheduling system designed to minimize worker fatigue through optimized job rotations in industrial settings. This project integrates fatigue modeling and combinatorial optimization to ensure fair, efficient, and health-conscious task assignments on the factory floor.

## 🚀 Project Overview

Physical fatigue can accumulate quickly in repetitive manufacturing environments, impacting both worker well-being and productivity. This tool was developed to dynamically assign tasks in a way that balances effort across shifts, minimizes injury risk, and improves long-term sustainability.

The project was implemented and evaluated in a real-world manufacturing environment at **Honda of Canada Manufacturing**, where it demonstrated measurable improvements in safety outcomes.

## 🎯 Key Features

- **Fatigue Modeling**: Captures how fatigue builds up over time based on task intensity and repetition.
- **Combinatorial Optimization**: Assigns workers to jobs using a cost-minimization algorithm that factors in both fatigue and task compatibility.
- **Scalable Design**: Supports integration into existing scheduling tools or ERP systems.
- **Custom Constraints**: Accommodates ergonomic limitations, skill levels, and mandatory rotation policies.

## 🛠 Tech Stack

- Python 3.x  
- NumPy / Pandas  
- PuLP (Linear Programming Solver)  
- Custom fatigue modeling function  
- Visualization tools (e.g., matplotlib, seaborn)

## 📊 Results

After deployment at Honda Plant 1 in Alliston, Ontario:
- ⚙️ 24% reduction in strain-related injuries over 6 months
- 📉 Decreased repetitive task exposure
- 📈 Improved worker satisfaction and retention

## 🔍 Example Use Case

```python
from scheduler import RotationOptimizer
optimizer = RotationOptimizer(worker_profiles, task_matrix, fatigue_weights)
optimal_schedule = optimizer.generate()
optimizer.visualize_schedule(optimal_schedule)
