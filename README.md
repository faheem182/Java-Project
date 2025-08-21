# Task Management API (Spring Boot)

A simple **Spring Boot REST API** for managing tasks.  
It supports basic **CRUD operations** (Create, Read, Update, Delete) using an **in-memory data structure**.

---

## 🚀 Features
- Create a task  
- Retrieve a task by ID  
- Retrieve all tasks  
- Update an existing task  
- Delete a task  

---

## 🗂 Project Structure

### **1. Task (Model)**
- Represents a task with fields: `id`, `title`, `description`, `status`.  
- Contains **getters, setters, and `toString()` method**.

### **2. Status (Enum)**
- Defines valid task statuses:  
  - `TODO`  
  - `IN_PROGRESS`  
  - `COMPLETED`  
  - `BLOCKED`

### **3. TaskService (Service Layer)**
- Acts as the **business logic layer**.  
- Stores tasks in a `Map<Long, Task>` (simulating a database).  
- Handles create, retrieve, update, delete operations.  

### **4. TaskController (REST Controller)**
- Exposes HTTP endpoints for task operations under `/tasks`.  
- Uses `@RestController` and `@RequestMapping`.  

---

## 📌 API Endpoints

| Method | Endpoint        | Description          |
|--------|-----------------|----------------------|
| POST   | `/tasks`        | Create a new task    |
| GET    | `/tasks/{id}`   | Get task by ID       |
| GET    | `/tasks`        | Get all tasks        |
| PUT    | `/tasks/{id}`   | Update a task        |
| DELETE | `/tasks/{id}`   | Delete a task        |

---

## 🛠 Testing with Postman

1. Open Postman → **Collections → + (New Collection)**  
2. Add a request for each operation below:  

### **POST – Create Task**
![POST Screenshot](https://github.com/My-Codes-21/160923733064-Mohammed_Sarfaraaz/blob/b5f24f48086361c98eb85ccaabbced42cd0a132b/post.png)

### **GET – Get All Tasks**
![GET Screenshot](https://github.com/My-Codes-21/160923733064-Mohammed_Sarfaraaz/blob/5d260ef213e83b1a872a57e9285f7feace6594ef/Get.png)

### **PUT – Update Task**
![PUT Screenshot](https://github.com/My-Codes-21/160923733064-Mohammed_Sarfaraaz/blob/5d260ef213e83b1a872a57e9285f7feace6594ef/PUT.png)

### **DELETE – Delete Task**
![DELETE Screenshot](https://github.com/My-Codes-21/160923733064-Mohammed_Sarfaraaz/blob/5d260ef213e83b1a872a57e9285f7feace6594ef/Delete.png)

---

## ✅ How to Run
1. Clone this repo:  
   ```bash
   git clone https://github.com/faheem182/my-project.git
   cd my-project
