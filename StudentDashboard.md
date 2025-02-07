### **📌 Assignment: Build a Student Dashboard with CRUD Operations**  

#### **🎯 Objective:**  
Create a **Student Dashboard** where users can **Add, Edit, Delete, and View** student details using **React + Redux** for the frontend and **FastAPI** for the backend.  

---

## **💡 Assignment Requirements**  

### **🔹 Backend (FastAPI)**
1. **Database:** Use **SQLite/PostgreSQL** to store student details.
2. **CRUD API Endpoints:**
   - **Create a student** (`POST /students/`)
   - **Read all students** (`GET /students/`)
   - **Read a single student** (`GET /students/{name}`)
   - **Update a student** (`PUT /students/{name}`)
   - **Delete a student** (`DELETE /students/{name}`)
3. **Student Model:**
   - `id`: Unique identifier (Auto-increment)
   - `name`: String (Required)
   - `age`: Integer (Required)
   - `email`: String (Unique)
   - `course`: String (Optional)

---

### **🔹 Frontend (React + Redux)**
1. **Create a Student Management Dashboard**
   - Display a **list of students**.
   - **Add a new student** using a form.
   - **Edit student details**.
   - **Delete a student** with confirmation.
2. **Use Redux for State Management**
   - Store student data in Redux.
   - Handle API calls with Redux Thunk or Redux Toolkit.
3. **Use Axios for API Calls**
   - Fetch student data from the FastAPI backend.
   - Perform **Create, Read, Update, Delete** operations.

---

### **🚀 Bonus Features (Optional)**
- **Search and Filter Students** by name, course, or age.
- **Pagination** to handle a large number of students.
- **Validation** for form fields (e.g., valid email format).
- **Material-UI/Tailwind for Styling**.

---

### **📌 Submission Requirements**
- **GitHub Repository** with both frontend and backend code.
- **README.md** explaining setup instructions.
- **Working API documentation (Swagger UI available in FastAPI by default).**

---

### **🔗 Example Endpoints**
| Method | Endpoint         | Description          |
|--------|-----------------|----------------------|
| GET    | `/students/`     | Get all students    |
| GET    | `/students/{name}` | Get a student by name|
| POST   | `/students/`     | Add a new student   |
| PUT    | `/students/{name}` | Update student info |
| DELETE | `/students/{name}` | Remove a student    |

---

### **⏳ Deadline**: _(Friday 07-02-2025)_
