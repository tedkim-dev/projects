# Mapsy Server - Appointment Booking System

## 📋 Project Overview

**Mapsy Server** is a comprehensive RESTful API service for managing appointments, vendors, designers, and customer interactions. The system facilitates appointment booking, and vendor-customer relationships for small business.

### 🎯 Key Features
- **Appointment Management**: Schedule and manage appointments
- **Vendor & Designer Management**: Handle vendor profiles, designer portfolios, and availability
- **Customer Experience**: Streamlined booking process with phone/email verification
- **Portfolio Showcase**: Display designer portfolios and services
- **Review System**: Customer feedback and rating system for items

### 📊 Project Details
- **Duration**: ~3.5 years of active development (April 2021 - November 2024)
- **Current Version**: 0.9.94
- **Status**: Production-ready with comprehensive test coverage

## 🏗️ Technical Architecture

### Technology Stack
- **Backend**: Go 1.22 with Gin framework
- **Database**: PostgreSQL 15.2 with GORM ORM
- **Authentication**: Supabase Auth + JWT tokens
- **File Storage**: Supabase Storage + AWS S3
- **Email Service**: Mailgun
- **SMS Service**: Twilio
- **Documentation**: Swagger/OpenAPI
- **Logging**: Uber Zap logger
- **Containerization**: Docker & Docker Compose

### Project Structure
```
mapsy-server/
├── api/                    # API types and schemas
├── cmd/                    # Application entry points
├── configs/               # Configuration management
├── database/              # Database layer
├── internal/              # Internal business logic
├── server/                # HTTP server implementation
├── templates/             # Email templates
└── docs/                  # API documentation
```

## 🚀 Key Achievements

### API Development
- Built comprehensive RESTful API with 20+ endpoints
- Implemented role-based access control (Admin/Guest)
- Designed scalable database schema with 5 core entities
- Achieved comprehensive test coverage for all endpoints

### Security & Performance
- Implemented JWT-based authentication with Supabase
- Added SMS-based phone verification system
- Configured rate limiting and CORS protection
- Optimized database queries and connection pooling

### Infrastructure
- Containerized application with Docker
- Set up CI/CD pipeline for automated testing
- Implemented structured logging and monitoring
- Deployed to staging and production environments

## 📚 API Endpoints

### Public Endpoints
- Vendor and designer listings
- Item catalog and category management
- Appointment booking system
- Customer registration and authentication

### Admin Endpoints
- User management and administration
- Content management (items, portfolios)
- Appointment oversight and management
- Analytics and reporting

## 🗄️ Database Design

### Core Entities
- **Vendors**: stores and businesses with contact information
- **Designers**: designers and craftsmen with portfolios
- **Appointments**: Customer booking sessions with scheduling
- **Items**: pieces and products with pricing
- **Users**: Customer accounts with authentication

## 🧪 Quality Assurance

### Testing Strategy
- Unit tests for business logic
- Integration tests for API endpoints
- Database migration testing
- Authentication flow testing

### Code Quality
- Comprehensive linting and code formatting
- API documentation with Swagger
- Error handling and logging
- Performance monitoring

## 📈 Deployment & Operations

### Environments
- **Development**: Local development with hot reload
- **Staging**: Pre-production testing environment
- **Production**: Live application with monitoring

### Monitoring
- Application health checks
- Database connectivity monitoring
- External service integration monitoring
- Performance metrics tracking

## 🤝 Development Process

### Workflow
- Feature branch development
- Code review and testing
- Automated CI/CD pipeline
- Documentation updates

### Standards
- Go coding conventions
- Conventional commit messages
- Comprehensive documentation
- Security best practices

---

**Last Updated**: November 2024  
**Version**: 0.9.94  