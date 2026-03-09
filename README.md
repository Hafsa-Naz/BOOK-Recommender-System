# Book Recommender System

## Project Overview
This project is a **Book Recommendation System built using Python**.  
It recommends books to users based on the ratings given by other users.

The system uses **Collaborative Filtering and Cosine Similarity** to find books that are similar to the one selected by the user. When a user enters a book name, the system suggests **4–5 similar books**.

---

## Dataset

The project uses the **Book-Crossing dataset**, which contains information about books, users, and their ratings.

### Files Used
- **Books.csv** – contains book titles, authors, and image links  
- **Ratings.csv** – contains ratings given by users  
- **Users.csv** – contains user information  

### Dataset Size
- **Books:** 271,360  
- **Users:** 278,858  
- **Ratings:** 1,149,780  

---

## Data Cleaning & Preprocessing

Before building the recommendation system, the dataset was cleaned and processed.

### Steps Performed
- Selected useful columns from the dataset
- Removed missing values
- Checked and removed duplicate records
- Merged ratings and book datasets using **ISBN**
- Filtered active users with more than **200 ratings**
- Selected books that have at least **50 ratings**

---

## Popularity-Based Recommendation

A **popularity-based recommender system** was created to display the **Top 50 most popular books**.

### Selection Criteria
- Number of ratings **≥ 250**
- Higher **average rating**

---

## Collaborative Filtering Recommendation

To recommend similar books, the following steps were used:

1. Created a **pivot table** of books and user ratings
2. Replaced missing values with **0**
3. Calculated similarity between books using **Cosine Similarity**
4. Selected the most similar books for recommendation

### Library Used

```python
from sklearn.metrics.pairwise import cosine_similarity
```

---

## Example Recommendation

### Example

```python
recommend("The Notebook")
```

### Output Example
- A Walk to Remember
- The Rescue
- One Door Away from Heaven
- Toxin

---

## Technologies Used

### Programming Language
- Python

### Libraries
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

### Tools
- Jupyter Notebook
- Git
- GitHub

---

## Future Improvements

- Build a **web interface using Streamlit**
- Add **content-based recommendation**
- Improve the **recommendation model**

---

## Author

**Hafsa Naz**  
BS Artificial Intelligence Student  
Dawood University of Engineering & Technology  

🔗 LinkedIn  
https://www.linkedin.com/in/hafsa-naz
