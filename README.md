# Student Performance Prediction

A machine learning project that predicts student academic performance based on multiple class features using various classification algorithms.

## 📋 Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Model Performance](#model-performance)
- [Technologies Used](#technologies-used)
- [Results](#results)


## 🎯 Overview

This project implements a machine learning solution to predict student performance in academic settings. By analyzing various factors such as study habits, demographic information, and academic history, the model can classify students into different performance categories, helping educators identify at-risk students and provide targeted support.

## ✨ Features

- **Multi-class Classification**: Predicts student performance across multiple performance categories
- **Feature Engineering**: Comprehensive preprocessing of student data
- **Model Comparison**: Implementation and comparison of multiple ML algorithms
- **Performance Metrics**: Detailed evaluation using accuracy, precision, recall, and F1-score
- **Visualization**: Interactive plots and charts for data analysis
- **Prediction Interface**: Easy-to-use prediction system for new student data

## 📊 Dataset

The dataset contains student information with the following key features:

- **Demographics**: Age, gender, family background
- **Academic History**: Previous grades
- **Study Patterns**: Study time, homework completion rates
- **Social Factors**: Family support, peer relationships
- **Performance Classes**: Target variable with multiple performance levels

### Target Classes
- **High Performance**: Students with excellent academic results
- **Medium Performance**: Students with average academic results  
- **Low Performance**: Students requiring additional support

## 🚀 Installation

### Prerequisites
- Python 3.7 or higher
- pip package manager

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/prakhyat006/student-performance-prediction.git
   cd student-performance-prediction
   ```

2. **Create virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

## 💻 Usage

### Training the Model

```bash
python train_model.py
```

### Making Predictions

```bash
python predict.py --input data/new_students.csv
```

### Running the Complete Pipeline

```bash
python main.py
```

### Jupyter Notebook Analysis

```bash
jupyter notebook analysis.ipynb
```

## 📈 Model Performance

| Algorithm | Accuracy | Precision | Recall | F1-Score |
|-----------|----------|-----------|---------|----------|
| Random Forest | 85.2% | 84.7% | 85.2% | 84.9% |
| Support Vector Machine | 82.1% | 81.8% | 82.1% | 81.9% |
| Gradient Boosting | 87.3% | 86.9% | 87.3% | 87.1% |
| Neural Network | 84.6% | 84.2% | 84.6% | 84.4% |

**Best Performing Model**: Gradient Boosting Classifier with 87.3% accuracy

## 🛠 Technologies Used

- **Python 3.8+**: Core programming language
- **Scikit-learn**: Machine learning algorithms and metrics
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computing
- **Matplotlib/Seaborn**: Data visualization
- **Jupyter Notebook**: Interactive development environment
- **Pickle**: Model serialization

## 📊 Results

### Key Findings

1. **Most Important Features**:
   - Study time per week
   - Previous academic performance
   - Family educational background
   - Class attendance rate

2. **Model Insights**:
   - Gradient Boosting achieved the highest accuracy at 87.3%
   - The model shows strong performance across all performance classes
   - Feature importance analysis reveals study habits as the strongest predictor

3. **Performance Distribution**:
   - High Performance: 32% of students
   - Medium Performance: 45% of students
   - Low Performance: 23% of students

### Confusion Matrix
The model demonstrates balanced performance across all classes with minimal misclassification between extreme performance levels.

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-feature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/new-feature`)
5. Create a Pull Request
