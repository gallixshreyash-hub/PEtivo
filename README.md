# PETIVO Experiment 5 Final

PETIVO is a React + Vite frontend connected to a Spring Boot backend using
Spring Data JPA and MySQL.

## What this version demonstrates

- React + Vite frontend
- Spring Boot REST API
- Spring Data JPA repository
- MySQL database persistence
- User/Admin login demonstration
- Appointment CREATE
- Appointment READ
- Appointment UPDATE
- Appointment DELETE

## Project structure

backend/
- Spring Boot API
- JPA entity and repository
- MySQL configuration

petivo-frontend/
- React/Vite interface
- Axios API calls
- Appointment booking/edit/delete UI

## Run it

See `RUN_ORDER.txt` for the exact live-demo sequence.

Backend:
    cd backend
    mvn spring-boot:run

Frontend (second terminal):
    cd petivo-frontend
    npm install
    npm run dev

Frontend:
    http://localhost:5173

Backend:
    http://localhost:8080

## Login credentials

User:
    user / user123

Admin:
    admin / admin123

## MySQL

Database:
    petivo_db

Default configuration:
    username: root
    password: root

If your MySQL password is different, edit:
`backend/src/main/resources/application.properties`

The JPA setting `spring.jpa.hibernate.ddl-auto=update` allows Hibernate to create/update
the `appointments` table from the Appointment entity.

## Assignment 4 relevance

The backend uses:
`AppointmentRepository extends JpaRepository<Appointment, Long>`

The appointment API demonstrates the four CRUD operations required for database
operations using a JPA Repository.

## Important

The sidebar/shop/order screens contain UI placeholders from the earlier frontend.
The database-backed feature implemented for this package is the appointment module.
