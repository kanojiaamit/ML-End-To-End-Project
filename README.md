# Student Performance Indicator

## Overview
This project implements an end-to-end machine learning solution for predicting student performance. The system utilizes various ML techniques and provides a user-friendly interface for making predictions, deployed on AWS Elastic Beanstalk.

## Key Features
- End-to-end ML pipeline with modular components
- Automated data ingestion and transformation
- Advanced model training using CatBoost
- Interactive web interface for predictions
- Automated CI/CD pipeline using GitHub Actions
- AWS cloud deployment

## Technologies Used
- **Programming Language:** Python
- **Development Environment:** VSCode
- **Data Processing & Analysis:**
  - Pandas
  - NumPy
  - Seaborn
  - Matplotlib
- **Machine Learning:**
  - scikit-learn
  - CatBoost
- **Model Serialization:** dill
- **Web Framework:** Flask
- **Cloud Platform:** AWS Elastic Beanstalk
- **CI/CD:** GitHub Actions

## Project Structure

```
MLEndToEnd/
│
├── .ebextensions/          # Elastic Beanstalk configuration
├── .git/                   # Git repository
├── artifacts/              # Model artifacts and outputs
├── catboost_info/         # CatBoost model information
├── logs/                   # Application logs
├── mlendtoend.egg-info/   # Package information
├── Notebook/              # Jupyter notebooks for EDA and modeling
│   ├── student_performance.ipynb        # EDA notebook
│   └── student_performance_modeling.ipynb # Model development notebook
├── src/                   # Source code
│   ├── components/        # Project components
│   ├── pipeline/         # ML pipelines
│   ├── utils.py          # Utility functions
│   ├── exception.py      # Custom exception handling
│   ├── logger.py         # Logging configuration
│   └── __init__.py       # Package initialization
│
├── templates/             # Web application templates
├── venv/                 # Virtual environment
├── app.py                # Main application file
├── application.py        # Application configuration
├── requirements.txt      # Project dependencies
├── setup.py             # Package setup configuration
└── .gitignore           # Git ignore rules
```

## Project Components

### 1. Data Science Pipeline
- **Data Ingestion:** Automated data loading and preprocessing
- **Data Transformation:** Feature engineering and scaling
- **Model Training:** Implementation of various ML algorithms
- **Model Evaluation:** Performance metrics and validation
- **Model Selection:** Best model selection based on metrics

### 2. Web Application
- Flask-based web interface
- Real-time prediction capabilities
- User-friendly input forms
- Responsive design

### 3. Development Resources
- Comprehensive EDA in `student_performance.ipynb`
- Model development process in `student_performance_modeling.ipynb`
- Modular code structure for maintainability

### 4. Deployment
- AWS Elastic Beanstalk hosting
- Automated deployments via GitHub Actions
- Logging and monitoring capabilities

## Setup and Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd MLEndToEnd
   ```

2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Install the package in development mode:
   ```bash
   pip install -e .
   ```

## Usage

### Local Development
1. Start the Flask application:
   ```bash
   python app.py
   ```
2. Access the web interface at `http://localhost:5000`

### Jupyter Notebooks
- For detailed EDA: Open `Notebook/student_performance.ipynb`
- For model development process: Open `Notebook/student_performance_modeling.ipynb`

## Model Training

The project uses various ML algorithms with a focus on CatBoost for optimal performance. The training pipeline includes:
1. Data preprocessing and cleaning
2. Feature engineering and selection
3. Model training and hyperparameter tuning
4. Performance evaluation and validation

## Deployment

### AWS Deployment
1. The application is deployed on AWS Elastic Beanstalk
2. Automated deployments are handled through GitHub Actions
3. Continuous monitoring and logging are implemented

### CI/CD Pipeline
- Automated testing on push
- Automated deployment to AWS
- Quality checks and validations

## Contributing
1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request
