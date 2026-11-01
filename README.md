# Setup Instructions

Follow these steps to set up and run the Community Issue Tracker project on your local machine.

## 1. Prerequisites

Install the following software:

- Java JDK
- Node.js and npm
- MySQL Server
- Git

## 2. Clone the Repository

Open a terminal and run:

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

Navigate to the project directory:

```bash
cd devops-project
```

## 3. Set Up the MySQL Database

1. Start the MySQL server.
2. Open MySQL Workbench.
3. Create the project database:

```sql
CREATE DATABASE community_issue_tracker;
```

4. Import or execute the project's SQL script to create the required tables, if provided.

## 4. Configure the Backend

Open the backend configuration file:

`backend/src/main/resources/application.properties`

Update the MySQL connection details:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/community_issue_tracker
spring.datasource.username=YOUR_MYSQL_USERNAME
spring.datasource.password=YOUR_MYSQL_PASSWORD
```

Replace the username and password with your local MySQL credentials.

## 5. Run the Backend

Open a terminal and navigate to the backend folder:

```bash
cd backend
```

Run the Spring Boot application on Windows:

```bash
mvnw.cmd spring-boot:run
```

The backend will run at:

`http://localhost:8080`

## 6. Run the Frontend

Open another terminal and navigate to the frontend folder:

```bash
cd client/my-react-app
```

Install the required dependencies:

```bash
npm install
```

Start the frontend application:

```bash
npm run dev
```

The frontend will normally run at:

`http://localhost:5173`

## 7. Access the Application

Open your web browser and visit:

`http://localhost:5173`

Make sure the MySQL server, Spring Boot backend, and React frontend are running.
 
# Admin login details
Email: admin@negombo.lk
Password: Admin123
