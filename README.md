# 🚗 Car Rental Platform (Spring Boot Project)

A full-stack **Car Rental Management System** built with **Spring Boot**, **Spring Data JPA**, **Spring Security**, **MySQL**, and **REST APIs**. This application allows users to browse cars, manage their own cars, make reservations, and handle user authentication.

---

## 📌 Features

### 🔐 Authentication & Security

* Password encryption with BCrypt
* User registration & login
* Spring Security integrated

### 🚘 Car Management

* Add, edit, delete cars
* List all available cars
* Upload car photos

### 📅 Reservations

* Reserve a car for specific dates
* Check availability
* Manage your reservations

### 🛢 Database

* MySQL with Hibernate & JPA
* Automatic table creation
* Entities:

  * `car_listings`
  * `my_cars`
  * `reservations`

### ⚙️ Backend Technologies

* Spring Boot 2.7.5
* Spring Data JPA
* Hibernate ORM
* Spring Security
* MySQL

---

## 🖥️ Requirements

* **Java JDK 20** (or newer)
* **Maven**
* **MySQL Server + Workbench**
* **VS Code** (with Java extensions) or IntelliJ IDEA

---

## 🔧 How to Run

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### 2️⃣ Configure MySQL

Create a database:

```sql
CREATE DATABASE car_rental;
```

### 3️⃣ Edit `application.properties`

Make sure the credentials match your MySQL:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/car_rental?useSSL=false&serverTimezone=UTC
spring.datasource.username=root
spring.datasource.password=yourpassword

spring.jpa.hibernate.ddl-auto=update
spring.jpa.database-platform=org.hibernate.dialect.MySQL5InnoDBDialect
```

### 4️⃣ Run the Application

Using VS Code or terminal:

```bash
mvn spring-boot:run
```

You will see:

```
Tomcat started on port(s): 8081
Started Demo20Application
```

👉 Open your browser:
**[http://localhost:8081/](http://localhost:8081/)**

---

## 🧱 Database Schema

### Tables Automatically Generated

* `car_listings`
* `my_cars`
* `reservations`
* Foreign keys & relations included

---

## 📁 Project Structure

```
src/main/java/com/example/demo20/
│
├── controller/
├── service/
├── model/
├── repository/
└── Demo20Application.java
```

---

## 📡 API Endpoints (Examples)

### Cars

| Method | Endpoint   | Description   |
| ------ | ---------- | ------------- |
| GET    | /cars      | Get all cars  |
| POST   | /cars/add  | Add a new car |
| DELETE | /cars/{id} | Delete a car  |

### Reservations

| Method | Endpoint      | Description           |
| ------ | ------------- | --------------------- |
| POST   | /reserve      | Make a reservation    |
| GET    | /reservations | Get user reservations |

---

## 🛠 Troubleshooting

### "Requires installing RedHat JDK extension" on VS Code

➡ Install the **Java Extension Pack**
➡ VS Code will automatically detect your JDK 20

### MySQL connection error

Check:

* Database name
* Username/password
* MySQL service is running

---

## 🤝 Contributing

Pull requests are welcome! For major changes, open an issue first.

---

## 📄 License

MIT License.

---

## 👤 Author

**Anteo Nebo**

If you want, I can also generate a **badge section**, **GIF previews**, or **API documentation**!
