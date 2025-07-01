# 📚 Book Recommender System
- A simple web-based Book Recommendation System using Flask, HTML, Bootstrap, and collaborative filtering. This project allows users to get personalized book recommendations based on input using content-based filtering and matrix factorization models.

# 🔍 Project Features
- Displays top 50 most popular books
- Recommends similar books using a collaborative filtering model
- Interactive web interface built using HTML and Bootstrap
- Backend powered by Flask
- Recommendation logic based on pre-computed similarity scores

# 🗂️ Project Structure
- ├── app.py                     # Flask app with routing and recommendation logic
- ├── index.html                 # Homepage template (Top 50 books)
- ├── recommend.html             # Recommendation page template
- ├── pouplar.pkl                # Pickled DataFrame of top-rated books
- ├── pt.pkl                     # Pivot table (user-book matrix)
- ├── books.pkl                  # Book metadata
- ├── similarity_scores.pkl      # Precomputed similarity matrix
- ├── BOOK-RECOMMENDATION(...)   # Jupyter notebook with Matrix Factorization model
- ├── Book Recommender System(...) # Jupyter notebook with Classification-based logic

# 🛠️ Tech Stack
- Frontend: HTML5, CSS3, Bootstrap 5
- Backend: Python, Flask
- ML Models: Matrix Factorization, Nearest Neighbors (precomputed)
- Libraries: NumPy, Pandas, Pickle

# 🧠 Recommendation Logic
- Top 50 Books: Displayed using popular_df data.
- User Input: When a book name is entered, similar books are found using the precomputed cosine similarity matrix.
- Output: Top 10 similar books with title, author, and image.

# ▶️ How to Run the Project Locally
1. Clone the repository: 
     git clone https://github.com/yadavsarang/Recommender-System-Using-Collaborative-Filtering.git
     cd Recommender-System-Using-Collaborative-Filtering
2. Install dependencies (create virtual environment recommended):
   pip install flask numpy pandas
3. Ensure the following .pkl files exist in the root directory:
- pouplar.pkl
- pt.pkl
- books.pkl
- similarity_scores.pkl
4. Run the app:
  python app.py
5. Open your browser and go to example- http://127.0.0.1:5000/

# 📒 Notebooks Included
Book Recommender System(CLF).ipynb: Implements a basic content-based filtering model.

BOOK-RECOMMENDATION(matrix factorization).ipynb: Demonstrates matrix factorization using collaborative filtering.

# 📌 To-Do (Suggestions)
 - Add user login & history tracking
 - Deploy on Render/Heroku
 - Improve search input with autocomplete
 - Add error handling for invalid book names

# Dataset:
  - https://www.kaggle.com/datasets/arashnic/book-recommendation-dataset
