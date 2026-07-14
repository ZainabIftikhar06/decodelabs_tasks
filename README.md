# DecodeLabs_internship
A collection of weekly AI projects developed during my 1-month AI internship at DecodeLabs.

### 📅 Week 1: Rule-Based AI Chatbot (The Logic Skeleton)
* **What was it?** Built an intelligent Rule-Based AI Chatbot focused on deterministic logic and control flow to process user inputs without relying on machine learning models.
* **How was it done?** 
  * Designed a Knowledge Base (KB) using Python dictionaries.
  * Implemented a continuous loop (heartbeat structure) to keep the chatbot live until an exit command is given.
  * Used string manipulation (`.lower()`, `.replace()`) and the `.get()` method for smooth input processing and exception handling.

### 📅 Week 2: Data Analytics & Product Classification (KNN Model)
* **What was it?** Implemented a data handling pipeline and applied supervised machine learning using the K-Nearest Neighbors (KNN) algorithm to classify product categories.
* **How was it done?**
  * Loaded and explored data using `pandas` to isolate key numeric features (`Quantity`, `UnitPrice`, `ItemsInCart`, `TotalPrice`).
  * Split the dataset into 80% training and 20% testing sets via `scikit-learn`.
  * Evaluated initial classification accuracy at `K=5` and optimized model performance by testing at `K=11`.
  * Visualized product trends and classification performance using a `matplotlib` and `seaborn` Confusion Matrix Heatmap.

📅 Week 3: AI Recommendation Logic (Tech Stack Recommender)

What was it? 
Built a content-based recommendation engine using TF-IDF vectorization and Cosine Similarity to match user skill profiles with the most relevant job roles.

How was it done?
Loaded and preprocessed job-role data using pandas to isolate key features (job_role, skills).
Converted user skills and job-role skill sets into weighted numerical vectors using TfidfVectorizer from scikit-learn.
Calculated similarity scores between the user profile and all job roles using cosine_similarity.
Built a 4-step ranking pipeline — Ingestion, Scoring, Sorting, Filtering — to return the Top-3 most relevant career path recommendations.
