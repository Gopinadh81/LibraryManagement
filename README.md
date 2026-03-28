library-management/
├── eureka-server/                  ← Service registry
├── api-gateway/                    ← Spring Cloud Gateway + JWT filter
├── user-service/
│   ├── src/main/java/com/library/user/
│   │   ├── controller/UserController.java
│   │   ├── service/UserService.java
│   │   ├── repository/UserRepository.java
│   │   ├── entity/User.java
│   │   ├── dto/LoginRequest.java, RegisterRequest.java, AuthResponse.java
│   │   ├── security/JwtUtil.java, SecurityConfig.java
│   │   └── UserServiceApplication.java
│   └── src/main/resources/application.yml
├── book-service/
│   ├── src/main/java/com/library/book/
│   │   ├── controller/BookController.java
│   │   ├── service/BookService.java
│   │   ├── repository/BookRepository.java
│   │   ├── entity/Book.java
│   │   ├── dto/BookRequest.java, BookResponse.java
│   │   └── BookServiceApplication.java
│   └── src/main/resources/application.yml
├── borrow-service/
│   ├── src/main/java/com/library/borrow/
│   │   ├── controller/BorrowController.java
│   │   ├── service/BorrowService.java
│   │   ├── repository/BorrowRepository.java
│   │   ├── entity/BorrowRecord.java
│   │   ├── client/UserClient.java       ← Feign
│   │   ├── client/BookClient.java       ← Feign
│   │   ├── dto/BorrowRequest.java
│   │   └── BorrowServiceApplication.java
│   └── src/main/resources/application.yml
├── notification-service/
│   ├── src/main/java/com/library/notification/
│   │   ├── consumer/BorrowEventConsumer.java  ← Kafka listener
│   │   ├── service/EmailService.java
│   │   ├── entity/Notification.java
│   │   └── NotificationServiceApplication.java
│   └── src/main/resources/application.yml
└── docker-compose.yml              ← MySQL + Kafka + Zookeeper
