# Todo Application

Spring Boot ile geliştirilmiş basit bir Todo uygulaması.



## 🛠️ Teknolojiler

- **Backend**: Spring Boot 3.5.4
- **Database**: MySQL 8.0
- **Template Engine**: Thymeleaf
- **Build Tool**: Maven
- **Java Version**: 21
- **ORM**: Spring Data JPA (Hibernate)

## 📋 Gereksinimler

- Java 21+
- MySQL 8.0+
- Maven 3.6+

## ⚙️ Kurulum

1. **Repository'yi klonlayın:**
   ```bash
   git clone https://github.com/sinankrkci/todoapp.git
   cd todoapp
   ```

2. **MySQL veritabanını oluşturun:**
   ```sql
   CREATE DATABASE todo_app;
   ```

3. **application.properties dosyasını düzenleyin:**
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/todo_app
   spring.datasource.username=your_username
   spring.datasource.password=your_password
   ```

4. **Uygulamayı çalıştırın:**
   ```bash
   mvn spring-boot:run
   ```

5. **Tarayıcıda açın:**
   ```
   http://localhost:8083
   ```

## 🗂️ Proje Yapısı

```
src/
├── main/
│   ├── java/
│   │   └── com/app/todoapp/
│   │       ├── controller/
│   │       │   └── TaskController.java
│   │       ├── models/
│   │       │   └── Task.java
│   │       ├── repository/
│   │       │   └── TaskRepository.java
│   │       ├── service/
│   │       │   └── TaskService.java
│   │       └── TodoappApplication.java
│   └── resources/
│       ├── templates/
│       │   └── tasks.html
│       └── application.properties
```

## 🔧 API Endpoints

- `GET /` - Ana sayfa (task listesi)
- `POST /` - Yeni task ekleme

## 📱 Kullanım

1. Ana sayfada yeni task eklemek için input alanına task başlığını yazın
2. "Add" butonuna tıklayın
3. Task otomatik olarak listeye eklenir



