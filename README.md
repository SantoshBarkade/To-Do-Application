# 📝 Spring Boot Todo Application

A simple **Todo web application** built with  
**Spring Boot**, **Thymeleaf**, **Bootstrap 5**, and **PostgreSQL**.

---

## ✨ Features
- Add new tasks
- Toggle tasks (mark as complete/incomplete)
- Delete tasks
- Display task creation date and time
- Responsive UI with Bootstrap 5

---

## 🛠️ Tech Stack
- **Backend:** Spring Boot, Spring Data JPA  
- **Frontend:** Thymeleaf, Bootstrap 5  
- **Database:** PostgreSQL  
- **Language & Tools:** Java 21, Maven

---

## 📋 Prerequisites
- Java 17 or higher  
- Maven installed  
- PostgreSQL installed and running locally (or via Docker)  

---

## 🚀 Installation / Setup

### 1. Clone the Repository
```bash
git clone https://github.com/<your-username>/springboot-todo-app.git
cd springboot-todo-app

2. Configure the Database

Create a PostgreSQL database and user:

CREATE DATABASE todo_app;
CREATE USER todo_user WITH PASSWORD 'strong_password';
GRANT ALL PRIVILEGES ON DATABASE todo_app TO todo_user;


Update src/main/resources/application.properties:

spring.datasource.url=jdbc:postgresql://localhost:5432/todo_app
spring.datasource.username=todo_user
spring.datasource.password=strong_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect

3. Build & Run
mvn spring-boot:run


Visit: http://localhost:8080
 in your browser.

🖥️ Usage

Add a new task in the input box and click Add.

Click Toggle to mark a task as complete/incomplete.

Click Delete to remove a task.

The task creation date is displayed beside each task title.

📂 Project Structure
src/
 ├─ main/java/.../controller   # Handles web requests
 ├─ main/java/.../service      # Business logic
 ├─ main/java/.../repository   # JPA repositories
 └─ main/resources/templates   # Thymeleaf templates

🖼️ Screenshots

Add screenshots of your UI here (optional).

💡 Future Enhancements

Add user authentication with Spring Security

Task categories or priorities

REST API endpoints for integration with mobile or frontend frameworks

Due dates & reminders

Docker containerization for easy deployment

🧑‍💻 Author

Santosh Sanjay Barkade

Feel free to fork, modify, and use this project as a starter template for your own Todo application.


---

This is **fully copy-ready**.  

You just need to:  
1. Save it as `README.md` in your project root.  
2. Replace `<your-username>` with your GitHub username.  
3. Commit & push:

```bash
git add README.md
git commit -m "Add README file"
git push
