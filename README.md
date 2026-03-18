# Fake Social Media Accounts Detection
<img src="https://i.postimg.cc/8PdzPc2b/Healthcare-AI-Credentialing-banner-2000x857-1.jpg" alt="FAKE SOCIAL MEDIA ACCOUNT DETECTION">

## Introduction
<p>
  Identifying fake social media accounts is a cumbersome task as malicious actors constantly evolve their techniques to mimic real human behavior. Changes in bot tactics make simple rule-based bans ineffective. In order to learn the specific characteristics of an inauthentic profile, we can use algorithms to identify structural and behavioral patterns through machine learning. Well-known algorithms for classification, such as Random Forest and Support Vector Machines (SVM), are able to process large datasets of account metadata, evaluating complex, non-linear relationships between features (like follower-to-following ratios, posting frequency, and profile completeness). These ML models are well-suited to tabular data and are able to process information step-by-step to predict whether an account is real or fake. The successful detection of fake accounts yields a safer, more trustworthy digital environment and protects users from misinformation and fraud.
</p>

## Aim
<p> 
  To predict and classify fake social media accounts according to profile metadata and behavioral data values using Machine Learning models.
</p>

## Objective
<p>
  The main objective of this project is to develop a web application that can detect inauthentic social media profiles based on real-time data inputs and provide a probability score of the account being a bot or sybil.  
</p>

## Project Scope
<p>
  The project has a wide scope, as it is not intended for a single social network but generalizes across common features found on platforms like Twitter, Instagram, and Facebook. This project is going to develop generic software, which can be applied by cybersecurity researchers, platform moderators, or everyday users. Moreover, it provides a facility to its users to compare the diagnostic results across different ML models (Random Forest, SVM, Logistic Regression) in real-time. 
</p>

## Key Features
- **Real-Time Classification:** Input an account's metrics and instantly receive a "Likely Fake" or "Likely Real" verdict.
- **Multiple ML Models:** Users can toggle between Random Forest, Decision Tree, Logistic Regression, and SVM to see how different algorithms evaluate the same data.
- **Risk Flagging:** The system highlights specific anomalies (e.g., "Suspicious Follower/Following Ratio" or "Missing Profile Picture") that contributed to the bot score.
- **Interactive Dashboard:** A modern, dark-mode GUI built with React and Tailwind CSS that displays recent global scans and system metrics.
  
## Technology Used:
- #### Languages:
  - ![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
  - ![CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
  - ![JAVASCRIPT](https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E)
  - ![PYTHON](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=darkgreen)
- #### FrameWork:
  - ![TAILWIND CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
  - ![REACT](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
- #### Machine-Learning Algorithms:
  - <a href="https://en.wikipedia.org/wiki/Random_forest">**RANDOM FOREST CLASSIFIER**</a>
  - <a href="https://en.wikipedia.org/wiki/Support_vector_machine">**SUPPORT VECTOR MACHINE (SVM)**</a>
  - <a href="https://en.wikipedia.org/wiki/Logistic_regression">**LOGISTIC REGRESSION**</a>
  - <a href="https://en.wikipedia.org/wiki/Decision_tree_learning">**DECISION TREE**</a>
- #### ML/DL:
  - ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
  - ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
  - ![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
- #### IDE:
  - ![VS Code](https://img.shields.io/badge/Visual_Studio_Code-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white)
  - ![Jupyter Notebook](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=white)
- #### OS used for testing:
  - ![MacOS](https://img.shields.io/badge/mac%20os-000000?style=for-the-badge&logo=apple&logoColor=white)
  - ![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
  - ![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)
## Overview

This project implements a machine learning solution to detect and classify fake social media accounts. It leverages multiple classification algorithms and provides an interactive web-based interface for real-time predictions.

**Definition**: A fake social media account is an inauthentic profile created for deception, spam, or manipulation, as opposed to genuine user accounts representing real individuals or legitimate organizations.
## Output Screen-shots

**1. Home Dashboard:** Displays real-time monitoring statistics, system status, and a live feed of recent global scans detecting potentially inauthentic accounts.
<img src="https://i.postimg.cc/9F9qPcvV/Screenshot-2026-03-18-192041.png" alt="Home Dashboard interface" width="50%">
<br><br>

**2. Analysis Engine (Detection Page):** The core interface where users input an account's metadata (followers, following, bio length, etc.) and select their preferred ML model for classification.
<img src="https://i.postimg.cc/3JGtc4yW/Screenshot-2026-03-18-192102.png" alt="Detection Input Form" width="50%">
<img src="https://i.postimg.cc/XNGLrGkk/Screenshot-2026-03-18-192110.png" alt="Detection Input Form" width="50%">
<br><br>

**3. Diagnostic Results:** Provides an instant verdict ("Likely Fake" or "Likely Real") along with a detailed Bot Probability Score and the specific behavioral risk flags that triggered the detection.
<img src="https://i.postimg.cc/ZqsPR49g/Screenshot-2026-03-18-192135.png" alt="Diagnostic Results Panel" width="50%">
<br><br>

**4. ML Infrastructure Page:** Offers transparency into the backend, detailing the accuracy, classification type, and characteristics of the Machine Learning algorithms (Random Forest, SVM, Decision Tree, Logistic Regression) powering the engine.
<img src="https://i.postimg.cc/ncf4MdzM/Screenshot-2026-03-18-192811.png" alt="Machine Learning Models Overview" width="50%">
## Key Components

1. **Pre-trained ML Models** — Four classification algorithms trained on labeled account data
2. **Streamlit Web Application** — Interactive user interface for model selection and predictions
3. **Jupyter Notebook** — Complete pipeline for exploratory data analysis, feature engineering, and model training
4. **Dataset** — Example fake and real user account data with extracted features

## Methodology & Workflow

### Data Pipeline
- **Data Preparation**: Raw account features are merged, cleaned, and preprocessed from CSV files
- **Feature Engineering**: Extraction and transformation of meaningful attributes from account metadata (e.g., profile characteristics, engagement patterns, account age)
- **Preprocessing**: Numerical scaling, categorical encoding, and handling missing values to prepare data for model input

### Machine Learning Models

Each model is trained using supervised learning with labeled examples (fake vs. real accounts):

- **Decision Tree** — A rule-based model that recursively splits data on features to make decisions; interpretable but prone to overfitting
- **Random Forest** — An ensemble of decision trees that reduces overfitting and improves robustness through majority voting
- **Logistic Regression** — A probabilistic linear classifier that outputs prediction confidence scores between 0 and 1
- **Support Vector Machine (SVM)** — A non-linear classifier that finds optimal decision boundaries in high-dimensional feature space

### Model Persistence

Models are serialized using **joblib**, a Python library for efficient saving/loading of sklearn objects. This allows trained models to be loaded and used for predictions without retraining.

## Repository Structure

```
.
├── streamlit_app.py                          # Interactive web application
├── Fake_social_media_acount_detection.ipynb  # Data exploration & model training notebook
├── decision_tree.joblib                      # Trained Decision Tree model
├── random_forest.joblib                      # Trained Random Forest model
├── logistic_regression.joblib                # Trained Logistic Regression model
├── svm_model.joblib                          # Trained SVM model
├── prediction_history.csv                    # Log of app predictions (auto-generated)
├── requirements.txt                          # Python dependencies
├── README.md                                 # This file
└── dataset/
    ├── fake_users.csv                        # Labeled fake account records
    └── real_users.csv                        # Labeled real account records
```

## Requirements

- **Python**: 3.8 or higher
- **Dependencies**: Listed in `requirements.txt`

Install all required packages:

```bash
pip install -r requirements.txt
```

## Getting Started

### Option 1: Interactive Web Application

1. Install dependencies (see above)
2. Navigate to the project directory
3. Run the Streamlit app:

```bash
streamlit run streamlit_app.py
```

4. Open your browser to the URL displayed (typically `http://localhost:8501`)
5. Select a model from the sidebar and enter account features to classify accounts as fake or real

### Option 2: Programmatic Use

Load and use a trained model directly in Python:

```python
import joblib
import pandas as pd

# Load a pre-trained model
model = joblib.load('random_forest.joblib')

# Prepare input data (must match training features and preprocessing)
# Example: X = pd.DataFrame({'feature1': [value], 'feature2': [value], ...})
# Ensure features are in the same order and format as used during training

# Make prediction
prediction = model.predict(X)  # Returns 0 (real) or 1 (fake)
probability = model.predict_proba(X)  # Returns confidence scores
```

**Important**: Input features must be preprocessed identically to the training data (scaling, encoding, feature order).

## Dataset Details

The `dataset/` folder contains two CSV files representing the training data:

- **fake_users.csv**: Account records labeled as inauthentic (fake = 1)
- **real_users.csv**: Account records labeled as authentic (real = 0)

**Usage**: These files serve as examples. To retrain models:
1. Merge both files
2. Apply feature engineering and preprocessing
3. Train models using sklearn
4. Export trained models with joblib

## Model Training & Retraining

The Jupyter notebook (`Fake_social_media_acount_detection.ipynb`) contains the complete training pipeline:

1. **Load & Explore**: Import and analyze fake/real user datasets
2. **Preprocessing**: Handle missing values, encode categorical variables, scale numerical features
3. **Feature Engineering**: Create or select relevant features for classification
4. **Model Training**: Train all four algorithms on the prepared dataset
5. **Evaluation**: Assess accuracy, precision, recall, and F1-score on test data
6. **Model Export**: Save the best-performing models using joblib

To retrain or experiment with new models:
- Open the notebook in Jupyter: `jupyter notebook Fake_social_media_acount_detection.ipynb`
- Modify preprocessing or feature engineering steps
- Run training cells and export updated models

## How the Application Works

1. **User Input**: User selects a model and provides account features via the Streamlit web interface
2. **Feature Preprocessing**: Input data is transformed (scaled, encoded) to match training data format
3. **Prediction**: The selected model classifies the account as fake or real
4. **Result Display**: Prediction and confidence score are shown to the user
5. **Logging** (optional): Prediction, input features, and timestamp are appended to `prediction_history.csv`

## Fake vs. Real Accounts: Key Differences in Society

### Real (Authentic) Accounts
**Characteristics**:
- Created by genuine individuals or legitimate organizations
- Consistent profile information (photo, bio, posting history)
- Natural engagement patterns with meaningful interactions
- Longer account history with gradual follower growth
- Original, authentic content reflecting real opinions and experiences
- Verified information (email, phone, identity verification where applicable)
- Balanced posting frequency and realistic interaction metrics

**Impact on Society**:
- Build genuine communities and authentic discourse
- Foster trust and transparency in social networks
- Enable real-world connections and meaningful relationships
- Support legitimate businesses and creators
- Contribute to informed public opinion and democratic participation

### Fake (Inauthentic) Accounts
**Characteristics**:
- Created with deceptive intent (often automated or purchased in bulk)
- Generic or stolen profile information and photos
- Unnatural engagement patterns (sudden spikes, bot-like behavior)
- Rapid follower accumulation or engagement without reciprocation
- Copy-pasted or AI-generated content with little originality
- Minimal or fabricated personal details
- Engagement primarily through automated interactions (likes, follows, comments)

**Impact on Society**:
- **Misinformation Spread**: Fake accounts amplify false narratives and conspiracy theories
- **Election Interference**: Coordinate inauthentic campaigns to influence political outcomes
- **Market Manipulation**: Artificially inflate engagement metrics for financial gain
- **Cyberbullying & Harassment**: Enable anonymous, consequence-free abuse
- **Fraud & Scams**: Used for phishing, romance scams, credential theft
- **Erosion of Trust**: Undermine confidence in social media platforms and online information
- **Mental Health Impact**: Contribute to social pressure and unrealistic expectations
- **Loss of Authentic Voice**: Drown out genuine user content with spam and propaganda

### Why Detection Matters
Detecting and removing fake accounts is critical for:
- **Platform Integrity**: Ensuring authentic user experience and trust
- **Public Health**: Combating health misinformation and dangerous trends
- **Economic Protection**: Preventing fraud and maintaining fair market competition
- **Democratic Integrity**: Protecting elections from manipulation
- **User Safety**: Reducing harassment, scams, and exploitation

## Common Workflow: Training New Models

```bash
# 1. Edit the notebook with new data or parameters
jupyter notebook Fake_social_media_acount_detection.ipynb

# 2. Run all cells to train models
# 3. Export new models (handled in notebook)

# 4. Test with the web app
streamlit run streamlit_app.py
```

## Contributing

We welcome contributions! Please follow these guidelines:

1. **Fork or Branch**: Create a feature branch for your changes
2. **Testing**: Include unit tests for preprocessing and prediction logic
3. **Documentation**: Update comments and docstrings for clarity
4. **Data Privacy**: Remove or anonymize any sensitive information before committing
5. **Pull Request**: Submit a PR with a clear description of changes and motivation


## Conclusion

The proliferation of fake social media accounts represents a critical challenge to the integrity of digital communities. This project provides a practical machine learning solution to combat this issue by leveraging multiple classification algorithms to identify inauthentic accounts with high accuracy.

### Key Takeaways

1. **Problem Significance**: Fake accounts cause real-world harm through misinformation, fraud, election interference, and erosion of public trust in digital platforms.

2. **Technical Approach**: By combining Decision Trees, Random Forests, Logistic Regression, and SVM models, this project demonstrates that fake accounts can be reliably detected through behavioral and profile analysis.

3. **Practical Applicability**: The Streamlit web interface makes this technology accessible to both technical and non-technical users, enabling widespread adoption for account verification and platform moderation.

4. **Future Improvements**: 
   - Integrate with real-time social media APIs for continuous monitoring
   - Incorporate deep learning models (LSTM, transformers) for advanced pattern detection
   - Extend to multi-platform detection across multiple social networks
   - Implement feedback loops to adapt models as fake account tactics evolve

5. **Responsible Use**: This tool should be used ethically to protect users and platforms, not to unfairly target legitimate accounts or infringe on privacy.

### Call to Action

If you are a platform developer, security researcher, or concerned citizen:
- Use this project as a foundation for your own detection systems
- Contribute improvements and feedback
- Help raise awareness about the dangers of inauthentic online activity
- Support policies and technologies that promote digital authenticity and trust

Together, we can build safer, more trustworthy online communities.

---

**Last Updated**: December 2025
**Version**: 1.0
