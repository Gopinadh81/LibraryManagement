library-management-system/          ← single GitHub repo
│
├── .github/
│   └── workflows/
│       └── ci.yml                  ← GitHub Actions (builds all services)
│
├── eureka-server/                  ← independent Spring Boot app
│   ├── src/
│   ├── pom.xml
│   └── Dockerfile
│
├── api-gateway/                    ← independent Spring Boot app
│   ├── src/
│   ├── pom.xml
│   └── Dockerfile
│
├── user-service/                   ← independent Spring Boot app
│   ├── src/
│   ├── pom.xml
│   └── Dockerfile
│
├── book-service/                   ← independent Spring Boot app
│   ├── src/
│   ├── pom.xml
│   └── Dockerfile
│
├── borrow-service/                 ← independent Spring Boot app
│   ├── src/
│   ├── pom.xml
│   └── Dockerfile
│
├── notification-service/           ← independent Spring Boot app
│   ├── src/
│   ├── pom.xml
│   └── Dockerfile
│
├── docker-compose.yml              ← spins up MySQL + Kafka + all services
├── .gitignore                      ← one file covers everything
└── README.md                       ← project overview
