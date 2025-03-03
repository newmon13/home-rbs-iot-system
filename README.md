# Home IoT Platform with Role-Based Access
![Java](https://img.shields.io/badge/Java-17-brightgreen)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.2.0-green)
![Python](https://img.shields.io/badge/Python-3.11-blue)
![Docker](https://img.shields.io/badge/Docker-Enabled-blue)
![License](https://img.shields.io/badge/License-MIT-yellow)

A comprehensive platform for managing IoT devices in a home environment with role-based access control, built with Java Spring for the backend and Python for device integration.

## Table of Contents
1. [About](#about)
2. [Features](#features)
3. [Architecture](#architecture)
4. [Technologies](#technologies)
5. [Getting Started](#getting-started)
6. [API Documentation](#api-documentation)
7. [Role-Based Access Control](#role-based-access-control)
8. [Device Integration](#device-integration)
9. [Contributing](#contributing)
10. [License](#license)

## About
This project provides a centralized platform to connect, manage, and automate various IoT devices within a home environment. The platform implements a robust role-based access control system, allowing different levels of access based on user roles (admin, family member, guest, etc.), ensuring security and privacy while maintaining ease of use.

## Features
Core functionality:
- [ ] Centralized device management and monitoring
- [ ] Role-based access control with customizable permissions
- [ ] Real-time device status updates
- [ ] Automated actions based on triggers and conditions
- [ ] Secure API for third-party integration

## Technologies
- **Backend**:
  - Java 17
  - Spring Boot 3.2.0
  
- **Device Integration**:
  - Python 3.11
  
- **Database**:
  - PostgreSQL
  
- **DevOps**:
  - Docker
  - Docker Compose
  
- **Testing**:
  - JUnit
  - Mockit
  - Testcontainers
  - pytest

## Getting Started
### Prerequisites
- Docker and Docker Compose
- Java 17 (for local development)
- Python 3.11 (for local development)
- PostgreSQL (optional for local setup)

### Running with Docker
1. Clone the repository:
```bash
git clone https://github.com/yourusername/home-iot-platform.git
```

2. Navigate to the cloned repository folder:
```bash
cd home-iot-platform
```

3. Start the application:
```bash
docker-compose up
```

The application will be available at http://localhost:8080
Admin dashboard will be accessible at http://localhost:8080/admin
API documentation will be available at http://localhost:8080/swagger-ui/index.html

## API Documentation
The API is fully documented using OpenAPI/Swagger. Once the application is running, you can access the documentation at:

http://localhost:8080/swagger-ui/index.html

## Role-Based Access Control
The platform implements a flexible role-based access control system with the following default roles:

- **Administrator**: Full access to all systems and configurations
- **Family Member**: Access to most devices and ability to create automations
- **Child**: Limited access to certain devices and restricted configuration abilities
- **Guest**: Temporary access to specific devices with time limitations
- **Device**: Special role for device-to-device communication

## License
This project is licensed under the MIT License - see the LICENSE file for details.
