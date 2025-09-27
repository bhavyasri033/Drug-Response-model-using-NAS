# Neural Architecture Search-Driven Optimization of Deep Learning Models for Drug Response Prediction

## Overview
This repository presents the implementation of Neural Architecture Search (NAS) techniques to optimize deep learning models for drug response prediction. Accurate prediction of drug responses is critical for personalized medicine, minimizing adverse effects, and enhancing therapeutic outcomes. Traditional deep learning models rely on manually designed architectures, which often struggle to capture the intricate relationships between genomic features and drug interactions.

To address this challenge, the project explores three NAS approaches—Random Search, Q-Learning, and Bayesian Optimization—to automatically identify optimal model architectures. Experimental results demonstrate that NAS-optimized models significantly outperform conventional deep learning methods, highlighting the role of automated architecture optimization in advancing personalized medicine.

## Published Work
- **Title:** Neural Architecture Search-Driven Optimization of Deep Learning Models for Drug Response Prediction  
- **Conference:** ICECMSN 2024  
- **Publisher:** Science Direct  
- **Sponsor:** Elsevier  
- [Read Research Paper](https://www.sciencedirect.com/science/article/pii/S1877050924034513)

## Features
- **Dataset:** PANCANCER_ANOVA from the Genomics of Drug Sensitivity in Cancer (GDSC) project  
- **NAS Search Strategies:** Random Search, Q-Learning, Bayesian Optimization  
- **Deep Learning Optimization:** Automatic architecture selection for better predictive performance  
- **Performance Evaluation:** MSE, MAE, R², RMSE metrics  
- **Model Deployment:** Flask API for drug response prediction  

## Dataset
The PANCANCER_ANOVA dataset contains 200,920 entries across 22 columns including:
- Drug Name, Drug ID, and Target Pathway  
- Gene Expression and Mutation Data  
- IC50 Values and Effect Sizes  
- False Discovery Rate (FDR) and P-values  

Sample data is included in the repository.

## Methodology

### Data Preprocessing
- Handling missing values  
- Feature scaling and normalization  
- Correlation analysis and feature selection  
- Dataset splitting for training, validation, and testing  

### Neural Network Architecture Design
- Defining the search space (layers, activations, dropout rates)  
- Hyperparameter tuning (learning rate, batch size, optimizer selection)  

### Neural Architecture Search Optimization
- **Random Search:** Randomly selects architectures for evaluation  
- **Q-Learning:** Uses reinforcement learning for guided architecture search  
- **Bayesian Optimization:** Uses probabilistic models for efficient exploration  

### Model Training and Evaluation
- Metrics: MSE, MAE, R², RMSE  
- Cross-validation and early stopping  
- Residual analysis for error interpretation  

### Model Deployment
- Flask API for drug response prediction  
- Scalable and integrable into biomedical applications  

## Results

| Method               | MSE       | R²        | MAE      | RMSE     |
|---------------------|-----------|-----------|----------|----------|
| Random Search       | 0.096292  | -0.003099 | 0.27427  | 0.310309 |
| Q-Learning          | 0.065483  | 0.116831  | 0.20684  | 0.255897 |
| Bayesian Optimization| 0.092374 | -0.069800 | 0.25340  | 0.303931 |

**Key Insights:**  
- Q-Learning performed best with the lowest error rates and highest R² score.  
- Bayesian Optimization showed moderate performance.  
- Random Search was the least effective, highlighting the need for guided optimization.  

## Conclusion & Future Scope
- Q-Learning-based NAS provides the most effective neural network architectures for drug response prediction.  
- Future work could explore:
  - Advanced NAS techniques (e.g., Evolutionary Algorithms, Reinforcement Learning)  
  - Expanding datasets with diverse drug compounds  
  - Explainability techniques for better interpretability  

## Installation & Usage

### Prerequisites
- Python 3.x  
- TensorFlow / PyTorch  
- Scikit-learn  

### Setup
1. Open Google Colab and load the notebook: [Open in Colab](#)  
2. Alternatively, run the notebook locally from repository files.  
3. Follow instructions to preprocess data, perform NAS optimization, and evaluate models.  

## Acknowledgments
- ICECMSN 2024 Conference for accepting this research  
- Science Direct for publication  
- Genomics of Drug Sensitivity in Cancer (GDSC) for the dataset  

## Citation
```bibtex
@article{G2025172,
  author={Uday Kiran G and Srilakshmi V and Padmini G and Sreenidhi G and Venkata Ramana B and Preetham Reddy G J},
  title={Neural Architecture Search-Driven Optimization of Deep Learning Models for Drug Response Prediction},
  journal = {Procedia Computer Science},
  volume = {252},
  pages = {172-181},
  year = {2025},
  note = {4th International Conference on Evolutionary Computing and Mobile Sustainable Networks},
  issn = {1877-0509},
  doi = {https://doi.org/10.1016/j.procs.2024.12.019},
  url = {https://www.sciencedirect.com/science/article/pii/S1877050924034513},
  keywords = {Neural Architecture Search, Random Search, Q-Learning, Bayesian Optimization, Drug Response Prediction}
}


## 🚀 Author
Bhavyasri Chapalamadugu  
[LinkedIn Profile](https://www.linkedin.com/in/bhavyasri-ch)
