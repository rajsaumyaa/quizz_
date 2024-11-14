# quizz_
# Quiz Platform

A robust web-based Quiz Platform built with Java EE, Maven, and MySQL, designed to run on Apache Tomcat server. This platform allows users to take quizzes and administrators to manage questions and answers.

## Features

### User Features
- User registration and authentication
- Take quizzes
- View quiz history and scores
- Track personal progress

### Admin Features
- Manage questions and answers
- Create new quizzes
- View user statistics
- Monitor quiz performance

## Technical Stack

- **Java EE**: Core programming language
- **Maven**: Dependency management and build tool
- **MySQL**: Database management
- **Apache Tomcat**: Application server
- **Eclipse IDE**: Development environment
- **JDBC**: Database connectivity

## Setup Instructions

1. **Prerequisites**
   - Java JDK 8 or higher
   - Maven 3.x
   - Eclipse IDE
   - Apache Tomcat 9.x
   - MySQL 8.x



2. **Project Setup**
   ```bash
   # Clone the repository
   git clone [repository-url]

   # Navigate to project directory
   cd quiz-platform

   # Build the project
   mvn clean install

   # Deploy to Tomcat
   # Copy the generated WAR file to Tomcat's webapps directory
   ```

3. **Configuration**
   - Update database credentials in `UserDAO.java`:
     ```java
     private String jdbcURL = "jdbc:mysql://localhost:30006/quiz_db";
     private String jdbcUserName = "root";
     private String jdbcPassword = "root";
     ```

## Project Structure

```
quiz-platform/
├── src/
│   └── main/
│       ├── java/
│       │   └── com/
│       │       └── user/
│       │           ├── dao/
│       │           │   └── UserDAO.java
│       │           └── model/
│       │               └── User.java
│       ├── resources/
│       └── webapp/
│           └── WEB-INF/
│               └── web.xml
├── pom.xml
└── README.md
```

## Usage

1. **User Registration**
   - Navigate to registration page
   - Enter username and password
   - Submit registration form

2. **Taking a Quiz**
   - Login with credentials
   - Select a quiz
   - Answer questions
   - Submit and view results

3. **Admin Panel**
   - Access admin dashboard
   - Manage questions and answers
   - View user statistics

## Security Features

- Password encryption
- Session management
- Input validation
- SQL injection prevention
- XSS protection

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Authors

- Saumya Raj - *Initial work*

## Acknowledgments

- Thanks to all contributors
- Special thanks to the open-source community
