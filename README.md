# GEBP
Green-Economic-Benefit-Prediction

# Green-Economic-Benefit-Prediction (GEBP)

## Project Title:  
**Digital Transformation Green Economic Benefit Prediction Based on Graph Neural Networks and Transformer**

### Overview:
This project implements a predictive framework for green economic benefits during digital transformation, using advanced deep learning methods. The model integrates **Graph Neural Networks (GNNs)**, **Transformer**, and **Reinforcement Learning (RL)** to accurately predict green economic benefits based on datasets such as WDI, GEM, GDP, and PWT 10.01. This approach outperforms traditional regression models and other deep learning methods, offering more precise support for decision-making in sustainable development.

### Data Availability Statement:
The data used in this study are publicly available. You can access the following datasets via the links below:

**World Development Indicators (WDI) dataset**: [Link](https://datacatalog.worldbank.org/search/dataset/0037712/World-Development-Indicators)
**Global Economic Monitor (GEM) dataset**: [Link](https://datacatalog.worldbank.org/search/dataset/0037798/Global-Economic-Monitor)
**Gross Domestic Product (GDP) dataset**: [Link](https://fred.stlouisfed.org/series/GDP)
**Penn World Table 10.01 (PWT 10.01)**: [Link](https://www.rug.nl/ggdc/productivity/pwt/)

### Experimental Environment:

#### Hardware Environment:
The experiments were conducted on a high-performance computing workstation equipped with:
AMD Ryzen 9 5950X @ 3.40GHz CPU
128GB DDR4 memory
Two NVIDIA RTX 3090 24GB GPUs

#### Software Environment:
**Programming Language**: Python
**Deep Learning Framework**: PyTorch

### Installation & Setup:
To set up the environment and run the code, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Liyan-C/GEBP.git
   cd GEBP
   ```

2. **Install required dependencies**:
   Make sure you have Python 3.8 or higher installed. Use the following command to install the necessary packages:
   ```bash
   pip install -r requirements.txt
   ```

### Code Usage:

1. **Data Preprocessing**:
   The datasets (WDI, GEM, GDP, PWT 10.01) are preprocessed in `data_preprocessing.py`:
   - Clean missing values
   - Normalize values
   - Split data into training and testing sets

2. **Model Training**:
   To train the model, run:
   ```bash
   python train.py --dataset [WDI | GEM | GDP | PWT]
   ```

3. **Evaluation**:
   To evaluate the trained model:
   ```bash
   python evaluate.py --model [trained_model_path] --dataset [WDI | GEM | GDP | PWT]
   ```

### Methodology:

#### Graph Neural Network (GNN):
The GNN is used to model complex relationships between various factors in the green economy, such as industrial chains and resource flows. By capturing dependencies between nodes, it enhances the accuracy and interpretability of the model.

#### Transformer:
The Transformer model captures long-term dependencies in the green economy transformation process through its self-attention mechanism, improving predictions on dynamic and time-series data.

#### Reinforcement Learning (RL):
The RL module dynamically adjusts decision-making strategies during the green economy transition, optimizing green economic benefits by maximizing cumulative rewards.

### Results:
Our model achieves significant improvements over traditional methods and other deep learning models in terms of prediction accuracy, as demonstrated by:
- **MSE**: Mean Squared Error (significant reduction)
- **MAE**: Mean Absolute Error (significant reduction)
- **R² Score**: Over 90% across all datasets


### License:
This project is licensed under the MIT License.
