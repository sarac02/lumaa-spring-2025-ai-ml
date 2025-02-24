### Movie Recommendation System (Content-Based)  

## Overview  
This is a **content-based recommendation system** that suggests movies based on a user's description.  
It utilizes **TF-IDF with cosine similarity** and an advanced **SBERT (Sentence Transformers) model** for better semantic matching.  

---

## Dataset  
- **Source**: [IMDb Dataset of Top 1000 Movies and TV Shows](https://www.kaggle.com/datasets/harshitshankhdhar/imdb-dataset-of-top-1000-movies-and-tv-shows)  
- **Steps to Load**:  
  - If using **Kaggle Notebook**, the dataset is available automatically.  
  - If running locally, **download** `imdb_top_1000.csv` from Kaggle and **place it in the project directory**.  

---

## Setup  
### **Python Version**  
- Recommended: **Python 3.8+**  

### **Install Dependencies**  
#### Install using `requirements.txt`:  
```bash
pip install -r requirements.txt
```
Manually install:
```bash
Copy
pip install pandas scikit-learn numpy sentence-transformers
```


### **Running the Code**
Option 1: Run in Kaggle Notebook
Open Kaggle Notebook and ensure the dataset is loaded.
Run all cells sequentially.
Get recommendations using:
recommend_movies("I love thrilling action movies set in space, with a comedic twist.")

Option 2: Run Locally in Jupyter Notebook
Open a terminal and start Jupyter Notebook:
Open ipynb file and run all cells.

Option 3: Run as a Python Script
Open a terminal in the project directory.
Run the script with a user input:
python recommend.py "I love thrilling action movies set in space, with a comedic twist."


## Output Example:
```bash
user_query = "I love thrilling action movies set in space, with a comedic twist."
```

Output:

| ID  | Title                          | Overview |
|-----|--------------------------------|------------------------------------------------------
| 538 | Amarcord                       | A series of comedic and nostalgic vignettes set in Italy. 
| 378 | The Incredibles                | A family of undercover superheroes fights against villains. 
| 692 | The Man Who Would Be King      | Two British former soldiers set themselves up as kings. 
| 826 | Barton Fink                    | A New York playwright is enticed to Hollywood. 
| 106 | Aliens                         | Fifty-seven years after surviving an alien apocalypse, Ripley returns. 

