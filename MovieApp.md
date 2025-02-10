### **Movie App Backend Assignment (TMDB Clone) 🎬 - FastAPI Edition**  

Your task is to **build a backend for a Movie App** that replicates **TMDB's features** using **FastAPI** with **MySQL or MongoDB**. This backend should support **movie data retrieval, searching, filtering, and watchlists** while maintaining high performance.  

---

## **🔹 Features to Implement**
### **1️⃣ Movie Data Management**
- **CRUD Operations:** Admins should be able to **add, update, and delete** movies.
- **Fetch Movies:** Users should be able to fetch **popular, trending, and upcoming movies**.
- **Search Movies:** Implement search by **title, genre, or cast**.

### **2️⃣ Advanced Filtering & Sorting**
- **Genre Filtering:** Allow users to filter movies by **genre, release date, or language**.
- **Sorting:** Sort movies by **popularity, rating, or release date**.

### **3️⃣ Movie Details & Reviews**
- **Movie Info:** Each movie should have **title, description, cast, genre, rating, and poster**.
- **Reviews & Ratings:** Users can **rate and review** movies.

### **4️⃣ Watchlist & Favorites**
- Users can **add movies to their watchlist** or **mark them as favorites**.

### **5️⃣ API Performance Optimization**
- **FastAPI Async Operations:** Use `async` functions for better scalability.
- **Database Indexing:** Optimize queries using **indexes on frequently searched fields**.
- **Redis Caching (Optional):** Improve response times by caching **popular queries**.

---

## **🔹 Tech Stack**
- **Backend:** FastAPI  
- **Database:** MySQL or MongoDB  
- **ORM:** SQLAlchemy (For MySQL) / Motor (For MongoDB)  
- **Caching (Optional):** Redis  
- **Deployment:** Host on **Render, DigitalOcean, or AWS**  

---

## **🔹 API Endpoints**
| **Method** | **Endpoint** | **Description** |
|-----------|-------------|----------------|
| **GET** | `/movies/` | Get all movies |
| **GET** | `/movies/{id}/` | Get single movie details |
| **POST** | `/movies/` | Add a new movie (Admin) |
| **PUT** | `/movies/{id}/` | Update movie (Admin) |
| **DELETE** | `/movies/{id}/` | Delete movie (Admin) |
| **GET** | `/movies/search/?q=title` | Search movies |
| **GET** | `/movies/filter/?genre=action` | Filter movies |
| **POST** | `/reviews/{movie_id}/` | Add a review |
| **POST** | `/watchlist/{movie_id}/` | Add to watchlist |

---

## **🔹 Assignment Deliverables**
✅ **Step 1**: Set up FastAPI & configure MySQL/MongoDB.  
✅ **Step 2**: Create movie models and define CRUD operations.  
✅ **Step 3**: Implement search, filtering, and sorting.  
✅ **Step 4**: Add watchlist & favorites functionality.  

---
