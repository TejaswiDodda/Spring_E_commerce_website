# 🛒 Spring E-Commerce Website

This is a fully functional **E-Commerce Website** built using **Spring MVC**, **Hibernate**, and **MySQL**. The application provides complete product management, user registration, and admin control features.

---

## 🆕 What's New

- 🔧 **Hibernate configuration added** — databases and tables auto-create on project run.
- ♻️ **Service classes** — reusable business logic across the application.
- 🗃️ **DAO classes** — handle direct interactions with the database.
- 🧩 **IDE Support** — compatible with both **IntelliJ IDEA** and **Eclipse**.

---

## 🚀 Quickstart

### 1. Clone the Repository
```bash
git clone https://github.com/TejaswiDodda/Spring_E_commerce_website.git
cd Spring_E_commerce_website
```

### 2. Open in Your IDE
- Open as a **Maven project**
- If using **IntelliJ IDEA**:
  - Open as **Spring Boot project**
  - Go to `Run > Edit Configurations...`
  - Set **Working Directory** to `$MODULE_WORKING_DIR$`

### 3. Configure Database
Update the following properties in `src/main/resources/application.properties`:
```properties
db.url=jdbc:mysql://localhost:3306/ecommjava?createDatabaseIfNotExist=true
db.username=your_username
db.password=your_password
```

> ⚠️ Tip: Avoid using `root` as your DB username for production. Ensure your user has appropriate privileges.

---

## 🔐 Login Credentials

After importing base data (via `basedata.sql`), use these:

- **Admin**  
  - Username: `admin`  
  - Password: `123`

- **User**  
  - Username: `lisa`  
  - Password: `765`

---

## 🏗️ Application Structure

```
Spring_E_commerce_website/
├── controller/        # Handles web requests and routes to views
├── dao/               # Database interaction layer
├── service/           # Business logic layer
├── entity/            # Data models / JPA entities
├── views/             # JSP files (web pages)
└── application.properties # Configuration file
```

### Example Route
```java
@GetMapping("/login")
public String adminLogin() {
    return "adminlogin"; // maps to src/main/webapp/views/adminlogin.jsp
}
```

---

## 🌐 Common Endpoints

- `/` → Home  
- `/register` → User Registration  
- `/admin/products` → Manage Products  
- `/admin/customers` → View Customers  
- `/admin/categories` → Product Categories  
- `/admin/Dashboard` → Admin Dashboard

---

## 🧠 Technologies Used

- **Spring MVC**
- **Spring Boot**
- **Hibernate**
- **MySQL**
- **JSP/Servlets**
- **Maven**

---

## 🗃️ Web Directory Configuration (For IntelliJ Users)

If views are not loading, set your working directory:
- Go to **Run > Edit Configurations...**
- Select `JtSpringProjectApplication`
- Modify working directory to: `$MODULE_WORKING_DIR$`
- Click Apply & OK


