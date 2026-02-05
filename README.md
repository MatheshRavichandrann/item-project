
# Item API – Spring Boot REST Application

This project is a simple **Spring Boot RESTful API** for managing a collection of items.  
It was developed as part of a **Freelance Java Developer sample task**.

---

## 🚀 Features

- Add a new item with input validation
- Retrieve an item by ID
- In-memory data storage using `ArrayList`
- Clean layered architecture (Controller → Service → Model)

---

## 🛠 Tech Stack

- Java 17  
- Spring Boot  
- Spring Web  
- Maven  

---

## 🔗 API Endpoints

| Method | Endpoint            | Description                | Request Body / Params           |
|--------|-------------------|----------------------------|--------------------------------|
| POST   | `/api/items`       | Add a new item             | JSON body with `name`, `price` |
| GET    | `/api/items/{id}`  | Retrieve item by ID        | Path variable `id`             |

**Example request for adding an item (POST `/api/items`):**

```json
{
  "name": "Laptop",
  "price": 45000
}
````

**Example request for getting an item (GET `/api/items/1`):**

```
GET https://item-project.onrender.com/api/items/1
```

---

## ▶️ How to Run Locally

1. Clone the repository:

```bash
git clone https://github.com/MatheshRavichandrann/item-project.git
cd item-project
```

2. Run the application:

```bash
mvn spring-boot:run
```

The API will be available at `http://localhost:8080`.

---

## 🌐 Deploy on Render

* Make sure your Spring Boot app **binds to the port provided by Render**:

```java
// application.properties
server.port=${PORT:8080}
```

* Push your code to GitHub
* Connect the repository to Render as a **Web Service**
* Render will automatically detect Spring Boot and d
* deploy your app

Your service will be available at a URL like:

```
https://item-project.onrender.com
```
