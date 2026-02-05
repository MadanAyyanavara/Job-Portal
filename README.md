# Job Portal

A full-stack job portal application that enables job seekers to search and apply for jobs with advanced filtering and ranking capabilities.

## Overview

Job Portal is a modern, cloud-ready web application built with cutting-edge technologies. It provides a seamless experience for job seekers to discover relevant job opportunities using real-time ranked full-text search powered by MongoDB Atlas Search.

## Key Features

- **Real-Time Ranked Full-Text Search**: Advanced search powered by MongoDB Atlas Search with intelligent ranking algorithms
- **Job Filtering & Discovery**: Filter jobs by location, experience level, salary range, and job category
- **User-Friendly Interface**: Responsive React.js frontend with intuitive design
- **Robust Backend API**: RESTful APIs built with Spring Boot for secure and efficient data handling
- **MongoDB Integration**: Custom aggregation pipelines and MongoDB Java Driver for optimized queries
- **API Documentation**: Comprehensive Swagger documentation for all endpoints
- **CORS-Enabled Communication**: Secure frontend-backend communication
- **Cloud-Ready Architecture**: Designed for AWS deployment with scalability in mind

## Tech Stack

### Frontend
- **React.js**: Modern JavaScript library for building user interfaces
- **HTML5 & CSS3**: Standards-based web technologies
- **JavaScript ES6+**: Modern JavaScript features

### Backend
- **Spring Boot**: Java-based framework for building enterprise applications
- **Java**: Core programming language
- **Spring Data & Spring Security**: For data access and authentication

### Database
- **MongoDB Atlas**: Cloud-based NoSQL database
- **MongoDB Java Driver**: Direct database connectivity
- **Custom Aggregation Pipelines**: Advanced data processing

### DevOps & Cloud
- **AWS**: Cloud infrastructure and deployment
- **Docker**: Containerization (optional)
- **Git**: Version control

### Documentation
- **Swagger/OpenAPI**: Interactive API documentation

## Project Structure

```
Job-Portal/
├── Frontend/          # React.js application
├── Backend/           # Spring Boot application
├── LICENSE            # MIT License
└── README.md          # This file
```

## Getting Started

### Prerequisites
- Node.js (v14+) and npm (for Frontend)
- Java 11+ (for Backend)
- MongoDB Atlas account
- AWS account (for deployment)

### Frontend Setup

1. Navigate to the Frontend directory:
   ```bash
   cd Frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm start
   ```
   The application will open at `http://localhost:3000`

### Backend Setup

1. Navigate to the Backend directory:
   ```bash
   cd Backend
   ```

2. Configure MongoDB Atlas credentials in `application.properties`

3. Build the project:
   ```bash
   mvn clean build
   ```

4. Run the Spring Boot application:
   ```bash
   mvn spring-boot:run
   ```
   The API will be available at `http://localhost:8080`

## API Documentation

Interactive API documentation is available via Swagger at:
```
http://localhost:8080/swagger-ui.html
```

Explore all available endpoints, request/response schemas, and test the APIs directly from the documentation.

## Database Schema

### Jobs Collection
- Job title, company, location
- Experience level, job type, salary range
- Job description and requirements
- Posted date and application deadline

### Indexed Fields for Search
- Job title (full-text)
- Company name
- Location
- Job description

## Features in Detail

### Search & Filtering
- Search jobs by keywords
- Filter by location, salary, and experience level
- Sort by relevance, date posted, or salary

### Application Management
- Submit job applications
- Track application status
- Save favorite jobs

## Deployment

### Deploy to AWS

1. **Frontend**: Deploy to AWS S3 + CloudFront
   ```bash
   npm run build
   # Upload build folder to S3
   ```

2. **Backend**: Deploy to AWS EC2 or Elastic Beanstalk
   ```bash
   mvn clean package
   # Deploy JAR to EC2/Beanstalk
   ```

3. **Database**: Use MongoDB Atlas (already cloud-hosted)

## Performance Optimizations

- MongoDB full-text search for fast job discovery
- Indexed queries for filtering operations
- Frontend caching and lazy loading
- API response pagination
- CORS optimization for frontend-backend communication

## Security Features

- Input validation and sanitization
- Spring Security for authentication
- CORS configuration for safe cross-origin requests
- Secure API endpoints

## Future Enhancements

- User authentication and profiles
- Advanced job recommendations
- Email notifications for new job matches
- Mobile app using React Native
- Employer dashboard for posting jobs
- AI-powered job matching

## Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues for bugs and feature requests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author

Developed by **Madan Ayyanavara**

## Support

For questions, issues, or suggestions, please open an issue on GitHub.

---

**Last Updated**: 2024
**Version**: 1.0.0
