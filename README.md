#  Stochastic Optimization for Recommendation Models

##  Project Description

This project compares several stochastic optimizers for training recommendation models. We apply **Adagrad**, **Adam**, **FTRL**, and **SGD** to recommendation systems based on **Matrix Factorization (MF)** and **Neural Collaborative Filtering (NCF)** using the **MovieLens 100k** dataset.

The goal is to evaluate the efficiency of each optimizer based on the following criteria: **prediction accuracy** (measured by RMSE and MAE), **training time**, and **scalability**.

---

##  Project Objectives

- **Optimizer Evaluation**: Compare Adagrad, Adam, FTRL, and SGD on recommendation tasks.
- **Methodology**: Implement both Matrix Factorization and Neural Collaborative Filtering (NCF).
- **Evaluation Metrics**:
  - Accuracy: RMSE, MAE  
  - Training time  
  - Scalability

---

##  Project Structure

![image](https://github.com/user-attachments/assets/cd0f15ca-c2e1-4280-a5c1-38226b6fdc01)

---

##  Dataset Used

We use the **MovieLens 100k** dataset: a collection of 100,000 ratings from 943 users on 1,682 movies.

- `u.data` : User ratings (userId, movieId, rating, timestamp)
- `u.item` : Movie metadata (title, genres, release year)
- `u.user` : User demographics (age, gender, occupation, zip code)

[Download MovieLens 100k Dataset](https://grouplens.org/datasets/movielens/100k/)

---

##  Technologies Used

The project is implemented using the following tools and libraries:

Python 3.x : Programming language

Pandas : Data manipulation and preprocessing

NumPy : Numerical computing

Matplotlib & Seaborn : Data visualization

Scikit-learn : Evaluation metrics (RMSE, MAE)

TensorFlow : Deep learning implementation (for NCF)

Optimizers : FTRL, Adam, Adagrad, SGD

---


## Project Installation Instructions

### 1. Download or Clone the Project

### 2. (Optional) Create and Activate a Virtual Environment

```bash
python -m venv env
source env/bin/activate  # On Windows: env\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

This will install all the required libraries, including:

* pandas
* numpy
* matplotlib
* scikit-learn
* tensorflow
* torch
* torch-optimizer

### 4. Launch the Jupyter Notebook

```bash
jupyter notebook projetoptimisation.ipynb
```

---

### Exemple
* Comparaison des Meilleurs Hyperparamètres : MF vs NCF :
* Les deux modèles ont été entraînés avec l'optimiseur Adam, en faisant varier les dimensions d’embedding, le taux d’apprentissage, le batch size et la régularisation.

![image](https://github.com/user-attachments/assets/a68513df-d256-4d0f-a823-9c1ae103dc95)

--- 

## Conclusion
* Ce projet permet de comparer des optimisations stochastiques appliquées à des modèles de recommandation, en tenant compte de plusieurs critères. Les optimisations appliquées incluent des méthodes classiques comme SGD, ainsi que des techniques plus récentes comme Adagrad ,Adam et FTRL.

