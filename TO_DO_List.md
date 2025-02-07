### **📌 Assignment: Build a To-Do List App with CRUD Operations**  

#### **🎯 Objective:**  
Create a **To-Do List Application** where users can **add, update, delete, and mark tasks as completed** using **React + Redux** for the frontend and **FastAPI** for the backend.  

---

## **💡 Assignment Requirements**  

### **🔹 Backend (FastAPI)**
1. **Database:** Use **SQLite/PostgreSQL** to store tasks.
2. **CRUD API Endpoints:**
   - **Create a Task** (`POST /tasks/`)
   - **Read all Tasks** (`GET /tasks/`)
   - **Read a single Task** (`GET /tasks/{title}`)
   - **Update a Task** (`PUT /tasks/{title}`)
   - **Delete a Task** (`DELETE /tasks/{title}`)
3. **Task Model:**
   - `id`: Unique identifier (Auto-increment)
   - `title`: String (Required)
   - `description`: String (Optional)
   - `completed`: Boolean (Default: False)

---

### **🔹 Frontend (React + Redux)**
1. **Create a To-Do Management Dashboard**
   - Display a **list of tasks**.
   - **Add a new task** using a form.
   - **Edit task details**.
   - **Delete a task** with confirmation.
   - **Mark a task as completed**.
2. **Use Redux for State Management**
   - Store task data in Redux.
   - Handle API calls with Redux Thunk or Redux Toolkit.
3. **Use Axios for API Calls**
   - Fetch task data from the FastAPI backend.
   - Perform **Create, Read, Update, Delete** operations.

---

### **🚀 Bonus Features (Optional)**
- **Filter Tasks** by status (Completed/Pending).
- **Sort Tasks** by priority or due date.
- **Drag and Drop Tasks** to reorder them.
- **Dark Mode Toggle**.
- **Material-UI/Tailwind for Styling**.

---

### **📌 Submission Requirements**
- **GitHub Repository** with both frontend and backend code.
- **README.md** explaining setup instructions.

---

### **🔗 Example Endpoints**
| Method | Endpoint       | Description            |
|--------|---------------|------------------------|
| GET    | `/tasks/`      | Get all tasks         |
| GET    | `/tasks/{title}`  | Get a task by ID      |
| POST   | `/tasks/`      | Add a new task        |
| PUT    | `/tasks/{title}`  | Update task info      |
| DELETE | `/tasks/{title}`  | Remove a task         |

---

### **⏳ Deadline**: _(08-02-2025)_  
