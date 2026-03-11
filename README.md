# 💬 Sentiment Analysis Project

## 🎯 Project Overview
This project addresses a common challenge in e-commerce: the manual analysis of thousands of daily product reviews. Manual processing is slow, costly, and difficult to scale. 

The goal of this project is to build a **Machine Learning model** capable of automatically classifying customer reviews into two categories:
* 😊 **Positive**
* 😡 **Negative**

By automating this process, the company can react faster to customer feedback, reduce operational costs, and prioritize negative reviews for the customer support team.

---

## 🚀 Key Features
* **Natural Language Processing (NLP):** Uses text processing techniques to handle product reviews.
* **Automated Classification:** Eliminates manual labor by categorizing sentiment with high efficiency.
* **Exploratory Data Analysis (EDA):** Includes deep dives into sentiment distribution and text characteristics.
* **Scalable Solution:** Built to handle large volumes of data as the e-commerce platform grows.

---

## 🛠️ Tech Stack & Libraries
This project is implemented in **Python** and utilizes the following libraries:
* **Data Manipulation:** `pandas`, `numpy`
* **Visualization:** `matplotlib`, `seaborn`
* **Machine Learning:** `scikit-learn` (Logistic Regression, TfidfVectorizer, Pipeline)
* **Model Storage:** `joblib`

---

## 📊 Methodology

### 1. Data Loading & EDA
The dataset consists of product reviews with key columns: `review_id`, `texto_review`, and `sentimento`. 
* **Initial Analysis:** Checking dimensions, sample data, and descriptive statistics.
* **Data Cleaning:** Identifying missing values and ensuring text consistency.

### 2. Preprocessing & Feature Engineering
* **TF-IDF Vectorization:** Converting raw text into numerical features that the model can understand.
* **Pipeline implementation:** Ensuring data transformations are consistent between training and testing.

### 3. Model Training
* **Algorithm:** Logistic Regression.
* **Optimization:** Using `GridSearchCV` for hyperparameter tuning to find the best performing model.
* **Persistence:** The final model is exported as a `.joblib` file for future use.

---

## 📈 Results
The model is evaluated using standard classification metrics:
* **Accuracy Score**
* **Confusion Matrix**
* **Classification Report** (Precision, Recall, and F1-Score)

---

## 💻 How to Use
1. **Clone the repository:** **_git clone https://urloftheproject_**
2. **Create a virtual environment: _python -m venv venv_**
3. **Instal the requirements.txt: _pip install -r requirements.txt_**
4. **if you use the jupyter notebook, maybe you will have to restart the venv sometimes.**

### A few tips for your setup:
* **The `.gitignore` file:** Make sure you have a `.gitignore` file in your project folder that includes `venv/`. You don't want to upload the entire virtual environment folder to GitHub, only the `requirements.txt` file.
* **Creating the requirements file:** If you haven't created the `requirements.txt` yet, you can do so by activating your environment and running:
    ```bash
    pip freeze > requirements.txt
    ```
* **Jupyter Kernel:** If you find that Jupyter doesn't "see" your virtual environment, you can manually add it as a kernel by running this inside the activated environment:
    ```bash
    pip install ipykernel
    python -m ipykernel install --user --name=venv --display-name "Python (Sentiment Project)"
    ```