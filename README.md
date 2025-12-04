# FitTrack — Fitness & Health Tracking App

A full-stack web application for tracking workouts, health metrics, and fitness goals.

## Tech Stack
- **Backend:** Spring Boot 3.2, Spring Security, JWT Authentication
- **Database:** PostgreSQL with JPA/Hibernate
- **Frontend:** React + TypeScript + Tailwind CSS
- **Docs:** OpenAPI/Swagger
- **Deployment:** Railway (backend), Vercel (frontend)

## Features
- 🔐 Secure authentication with JWT tokens
- 🏋️ Log workouts with exercises, sets, reps, and weights
- 📊 Track health metrics (weight, sleep, mood)
- 📈 Dashboard with workout streaks and progress trends
- 📱 Responsive design

## API Documentation
Interactive API docs available at `/swagger-ui.html`

## Architecture
```
src/
├── controller/    # REST endpoints
├── service/       # Business logic
├── repository/    # Data access
├── entity/        # JPA entities
├── dto/           # Request/response objects
├── security/      # JWT & auth config
└── exception/     # Error handling
```

## Running Locally
```bash
# Start PostgreSQL
docker-compose up -d db

# Run backend
./mvnw spring-boot:run

# Run frontend
cd frontend && npm run dev
