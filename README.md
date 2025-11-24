# Beginner Machine Learning Projects

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

This repository contains the final submission for the **Beginner Machine Learning** course from Dicoding. The project implements two machine learning approaches: **Clustering** and **Classification**.

## 📚 Table of Contents

- [About The Project](#about-the-project)
- [Project Structure](#project-structure)
- [Dataset](#dataset)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Results and Analysis](#results-and-analysis)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## 🎯 About The Project

This project demonstrates the implementation of two fundamental machine learning techniques:

### 1. **Clustering (Unsupervised Learning)**
Uses clustering algorithms to group unlabeled data. This technique is useful for:
- Customer segmentation
- Data pattern analysis
- Anomaly detection
- Data exploration

### 2. **Classification (Supervised Learning)**
Uses classification algorithms to predict categories or classes from data based on existing features. This technique is useful for:
- Category prediction
- Automated decision making
- Pattern recognition
- Predictive analysis

## 📁 Project Structure

```
proyek-machine-learning-pemula/
│
├── README.md
│   └── Project documentation
│
├── [Clustering]_Submission_Akhir_BMLP_MC009d5X2352 (2).ipynb
│   └── Main notebook for clustering analysis
│
├── [Klasifikasi]_Submission_Akhir_BMLP_MC009D5X2352 (4).ipynb
│   └── Main notebook for classification analysis
│
├── Clustering/
│   ├── data_clustering (2).csv
│   │   └── Dataset for clustering
│   ├── data_clustering_inverse (6).csv
│   │   └── Inverse transformed dataset
│   ├── model_clustering (2).h5
│   │   └── Saved clustering model
│   └── PCA_model_clustering (1).h5
│       └── PCA model for dimensionality reduction
│
└── Klasifikasi/
    ├── decision_tree_model (2).h5
    │   └── Decision Tree model
    ├── explore_LogisticRegression_classification (2).h5
    │   └── Logistic Regression model
    └── tuning_classification (3).h5
        └── Hyperparameter tuned model
```

## 📊 Dataset

This project uses datasets suitable for each technique:

### Clustering
- `data_clustering (2).csv` - Main dataset for clustering analysis
- `data_clustering_inverse (6).csv` - Inverse transformed dataset from normalization process

### Classification
- Dataset for classification (embedded in notebook or automatically downloaded)

> **Note**: Clustering datasets are already available in the repository. Make sure the dataset paths are correct when running the notebooks.

## 🛠️ Technologies Used

### Programming Language
- Python 3.8+

### Libraries
- **Data Processing**:
  - NumPy
  - Pandas
  
- **Visualization**:
  - Matplotlib
  - Seaborn
  
- **Machine Learning**:
  - Scikit-learn
  - TensorFlow/Keras (for save/load .h5 models)
  
- **Development**:
  - Jupyter Notebook

## 🚀 Installation

### 1. Clone Repository

```bash
git clone https://github.com/maaulidna/proyek-machine-learning-pemula.git
cd proyek-machine-learning-pemula
```

### 2. Create Virtual Environment (Optional but Recommended)

```bash
# Windows
python -m venv venv
venv\Scripts\activate

# Linux/Mac
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install numpy pandas matplotlib seaborn scikit-learn jupyter tensorflow
```

> **Note**: TensorFlow/Keras is required for loading .h5 model files

Or if you have a requirements.txt file:

```bash
pip install -r requirements.txt
```

## 💻 Usage

### Running Notebooks

1. Open Jupyter Notebook:
```bash
jupyter notebook
```

2. Select the notebook you want to run:
   - `[Clustering]_Submission_Akhir_BMLP_MC009d5X2352 (2).ipynb` for clustering analysis
   - `[Klasifikasi]_Submission_Akhir_BMLP_MC009D5X2352 (4).ipynb` for classification analysis

3. Run cells sequentially (Shift + Enter)

### General Workflow

#### For Clustering:
1. **Data Loading**: Import and load dataset
2. **Exploratory Data Analysis (EDA)**: Analyze and visualize data
3. **Data Preprocessing**: Cleaning, normalization, and transformation
4. **Clustering**: Implement algorithms (K-Means, DBSCAN, etc.)
5. **Evaluation**: Evaluate using metrics like Silhouette Score, Elbow Method
6. **Visualization**: Visualize resulting clusters

#### For Classification:
1. **Data Loading**: Import and load dataset
2. **Exploratory Data Analysis (EDA)**: Analyze class and feature distribution
3. **Data Preprocessing**: Feature engineering, encoding, scaling
4. **Train-Test Split**: Split data into training and testing sets
5. **Model Training**: Train classification models
6. **Evaluation**: Evaluate using accuracy, precision, recall, F1-score
7. **Prediction**: Make predictions on new data

## 📈 Results and Analysis

### Clustering
The clustering project implements various techniques:

- **Dimensionality Reduction**: Using PCA (Principal Component Analysis)
  - Model: `PCA_model_clustering (1).h5`
  - Purpose: Reduce feature dimensions for visualization and computational efficiency

- **Clustering Model**: 
  - Saved model: `model_clustering (2).h5`
  - Produces data groupings based on discovered patterns
  
- **Output Dataset**:
  - `data_clustering_inverse (6).csv` - Inverse transformed data for interpretation

### Classification
The classification project explores multiple algorithms:

- **Decision Tree**:
  - Model: `decision_tree_model (2).h5`
  - Tree-based algorithm for classification

- **Logistic Regression**:
  - Model: `explore_LogisticRegression_classification (2).h5`
  - Linear classification algorithm

- **Hyperparameter Tuning**:
  - Model: `tuning_classification (3).h5`
  - Optimized hyperparameter model for best performance

> **Note**: All models are saved in .h5 format for easy deployment and reusability.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/maaulidna/proyek-machine-learning-pemula/issues).

### How to Contribute:

1. Fork this repository
2. Create a new branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Create a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Contact

**Maulidna**

- GitHub: [@maaulidna](https://github.com/maaulidna)
- Project Link: [https://github.com/maaulidna/proyek-machine-learning-pemula](https://github.com/maaulidna/proyek-machine-learning-pemula)

## 🙏 Acknowledgments

- [Dicoding Indonesia](https://www.dicoding.com/) - Learning platform
- [Scikit-learn Documentation](https://scikit-learn.org/) - ML algorithm reference
- All contributors who have helped this project

---

⭐ Don't forget to give a star if this project helps you!

**#MachineLearning #Python #DataScience #Dicoding**
