# Process Mining and Automata Learning: Controllability Analysis

## 🎯 Project Overview

This project implements a comprehensive solution for **Process Mining and Automata Learning** with a focus on evaluating controllability of extracted processes. The project is structured around three main assignments that progressively build upon each other to create a complete process mining analysis pipeline.

## 📋 Assignment Structure

### Assignment 1: Extracting the Markov Process from a Log
- **Objective**: Extract Petri Nets from event logs and build Markov processes
- **Key Components**:
  - Petri Net extraction using process mining algorithms
  - Trace alignment between logs and Petri Nets
  - Automata learning wrapper implementation
  - State transition analysis

### Assignment 2: Calculating Entropy and Information Gain
- **Objective**: Analyze process predictability through entropy measures
- **Key Components**:
  - State entropy calculations
  - Process-level entropy analysis
  - Information gain computation for trace tests
  - Uncertainty quantification

### Assignment 3: Trace Test Relabeling and Entropy Analysis
- **Objective**: Transform logs using trace tests and analyze controllability
- **Key Components**:
  - Trace test relabeling procedures
  - Comparative entropy analysis
  - Process controllability evaluation
  - Optimization strategies

## 🛠️ Technical Implementation

### Core Technologies
- **Python 3.8+**: Primary programming language
- **PM4Py**: Process mining library for Petri Net extraction and analysis
- **NetworkX**: Graph analysis and visualization
- **Matplotlib/Seaborn/Plotly**: Advanced visualizations
- **NumPy/SciPy**: Mathematical computations
- **Pandas**: Data manipulation and analysis

### Key Features
- ✅ Complete mathematical formulation implementation
- ✅ Beautiful interactive visualizations
- ✅ Comprehensive entropy analysis
- ✅ State-of-the-art process mining algorithms
- ✅ Detailed documentation and explanations
- ✅ All-in-one Jupyter notebook implementation
- ✅ Automatic results saving and organization

## 📁 Project Structure

```
process_mining/
├── README.md                          # Project documentation
├── requirements.txt                   # Python dependencies
├── process_mining_complete.ipynb      # Main Jupyter notebook (All code & analysis)
├── #Assignment 2 - pm.pdf            # Assignment requirements
└── results/                           # Generated outputs and analysis
    ├── data/                          # Generated data files
    │   ├── alignment_quality_stats.json
    │   ├── alignment_results.json
    │   ├── learning_episode_simulation.json
    │   ├── log_statistics.json
    │   ├── markov_process_data.json
    │   ├── petri_net_statistics.json
    │   └── synthetic_event_log.csv
    ├── models/                        # Saved models and pickled objects
    │   ├── automata_learning_wrapper.pickle
    │   ├── markov_process_builder.pickle
    │   ├── markov_transition_probabilities.pickle
    │   ├── markov_transitions.pickle
    │   ├── petri_net_inductive.pickle
    │   ├── petri_nets_all_algorithms.pickle
    │   └── trace_alignments.pickle
    └── plots/                         # Generated visualizations
        ├── assignment1/               # Assignment 1 plots and diagrams
        └── exploratory/               # Exploratory analysis visualizations
```

## 🚀 Getting Started

### Prerequisites
- Python 3.8 or higher
- Jupyter Notebook or JupyterLab
- Graphviz (for Petri Net visualization)

### Installation

1. **Navigate to the project directory**
   ```powershell
   cd "d:\University\4th Semester\2. BDSS\assignments\2. process_mining"
   ```

2. **Install dependencies**
   ```powershell
   pip install -r requirements.txt
   ```

3. **Install Graphviz** (for Petri Net visualization)
   - Windows: Download and install from https://graphviz.org/download/
   - macOS: `brew install graphviz`
   - Linux: `sudo apt-get install graphviz`

4. **Launch Jupyter Notebook**
   ```powershell
   jupyter notebook
   ```

5. **Open the main notebook**
   - Navigate to `process_mining_complete.ipynb`
   - This notebook contains all the code, analysis, and documentation for the three assignments

## 💡 Usage

The entire project is implemented in a single, comprehensive Jupyter notebook:
- **`process_mining_complete.ipynb`**: Contains all assignments with complete implementations
- All code is modular and well-documented within the notebook
- Results are automatically saved to the `results/` directory
- Generated models, data, and visualizations are preserved for analysis

## 📊 Key Mathematical Formulations

### State Entropy
```
H(Q) = -∑[P(Q→Qi) × log₂(P(Q→Qi))]
```

### Process Entropy
```
H(Process) = ∑[P(Q) × H(Q)]
```

### Information Gain
```
IG = H(Process) - H(TraceTest)
```

## 🎨 Visualization Features

- **Interactive Petri Net diagrams** with state highlighting
- **Markov process state transition graphs** with probability annotations
- **Entropy heatmaps** showing process uncertainty
- **Information gain charts** for trace test analysis
- **Timeline visualizations** for trace alignment
- **3D process landscapes** for complexity analysis

## 📈 Expected Outcomes

1. **Complete Markov Process Extraction**: From raw event logs to fully annotated Markov models
2. **Comprehensive Entropy Analysis**: Quantitative measures of process predictability
3. **Optimized Trace Test Strategies**: Data-driven approaches for process control
4. **Visual Process Insights**: Clear, beautiful visualizations of complex process behaviors
5. **Reproducible Research**: Well-documented, modular code for academic use

## 🔬 Research Applications

This project provides a foundation for:
- **Process Optimization**: Identifying bottlenecks and improvement opportunities
- **Predictive Process Analytics**: Forecasting process outcomes
- **Compliance Monitoring**: Detecting deviations from expected behavior
- **Resource Allocation**: Optimizing human and computational resources
- **Quality Control**: Ensuring process consistency and reliability

## 📚 References

- Pietro Sala, "Process Mining and Automata Learning: evaluate controllability of extracted processes"
- Biomedical Decision Support Systems 24/25 Course Materials
- PM4Py Documentation and Process Mining Handbook

## 👤 Author

**Emil Alizada**  
*Biomedical Decision Support Systems Course*  
*4th Semester, 2025*

## 🤝 Contributing

This project is part of academic coursework. The implementation is contained within the main Jupyter notebook for easy review and execution. For questions or improvements:
1. Document any issues or enhancement ideas
2. Follow the established code structure within the notebook
3. Ensure all mathematical formulations are properly implemented
4. Test any modifications thoroughly within the notebook environment

## 📄 License

This project is for educational purposes as part of the Biomedical Decision Support Systems course.

---

**Author**: Emil Alizada  
**Course**: Biomedical Decision Support Systems  
**Status**: ✅ Complete | **Last Updated**: July 21, 2025
