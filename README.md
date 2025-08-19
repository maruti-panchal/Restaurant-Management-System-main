# 🍴 Restaurant Management System

A Spring Boot application to manage restaurant operations with role-based access control.  
Admins can manage users and menu items, while users can sign up, log in, browse the menu, and place orders.  
Visitors can view the menu without signing in.

---

## 🚀 Features

- **Role-based access** – Admin, User, Visitor
- **User Management** – Signup, Signin, Authentication
- **Food Menu Management** – Add and view food items
- **Order Management** – Place and track orders
- **Email Notifications** – Sent using JavaMail API
- **Secure APIs** – Authentication and authorization with Spring Security
- **API Documentation** – Swagger UI integration

---

## 🛠 Tech Stack

- **Backend:** Spring Boot, Java 21
- **Database:** MySQL
- **Build Tool:** Maven
- **Security:** Spring Security, JWT/Auth Tokens
- **Docs:** SpringDoc OpenAPI (Swagger UI)
- **Email:** JavaMail API

---

## 🗄 Database Design

### **User Table**

- `id`, `username`, `password`, `email`, `role`, `is_signed_up`, `is_signed_in`, `created_at`

### **Food Item Table**

- `id`, `name`, `description`, `price`, `type`

### **Order Table**

- `id`, `user_id`, `food_item_id`, `status`, `order_date`

---

## 📦 How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/restaurant-management-system.git

   ```

2. Configure MySQL in application.properties:

spring.datasource.url=jdbc:mysql://localhost:3306/restaurant_db
spring.datasource.username=root
spring.datasource.password=yourpassword

3. Run the project:

mvn spring-boot:run

4. Access Swagger UI:

http://localhost:8080/swagger-ui.html
