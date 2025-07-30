# Tamp - Digital Loyalty Platform REST API

## Project Overview
**Tamp** is a comprehensive digital loyalty platform that enables businesses to create and manage digital stamp cards, while allowing customers to collect stamps and redeem rewards through a modern REST API. The system replaces traditional paper-based loyalty programs with a scalable, cloud-native solution.

## Key Features
- **Digital Stamp Cards**: Businesses can create customizable stamp card templates with configurable redemption conditions
- **NFC Integration**: Physical NFC stamps for seamless in-store stamp collection
- **Multi-Reward System**: Support for multiple redemption points within a single stamp card
- **Geolocation Services**: Location-based business discovery and nearby company search
- **Notification System**: Automated user notifications for stamp collection progress and redemption opportunities (stored in database, retrieved via API)
- **User Management**: Complete user lifecycle management with Supabase authentication
- **Company Management**: Business profile management with metadata, locations, and stamp templates

## Technical Architecture

### Backend Stack
- **Language**: Go 1.24 (Golang)
- **Framework**: Chi HTTP router for RESTful API endpoints
- **Database**: PostgreSQL with PostGIS for geospatial data
- **Authentication**: Supabase Auth integration
- **API Documentation**: OpenAPI 3.0 specification with auto-generated code
- **Database Migrations**: Goose migration tool
- **Logging**: Structured logging with Go's standard slog package

### Core Technologies
- **HTTP Router**: Chi v5 for high-performance routing
- **Database ORM**: SQLx for enhanced database operations
- **Code Generation**: oapi-codegen for OpenAPI-driven development
- **Configuration**: Environment-based configuration management
- **Error Handling**: Custom error types with structured error responses
- **Middleware**: CORS, authentication, logging, and request tracing

### Database Design
- **Relational Schema**: Normalized PostgreSQL database with 15+ migration files
- **Geospatial Support**: PostGIS integration for location-based queries
- **JSON Storage**: Flexible metadata storage using PostgreSQL JSONB
- **Audit Trail**: Comprehensive created_at/updated_at timestamps
- **Soft Deletes**: Status-based record management

## Key Components

### Core Entities
- **Companies**: Business profiles with locations, metadata, and stamp templates
- **Coupons**: User-specific stamp cards with progress tracking
- **Coupon Templates**: Reusable stamp card configurations
- **Company Stamps**: Physical NFC stamps linked to businesses
- **Redemptions**: Reward redemption tracking and validation
- **Users**: Customer accounts with onboarding status tracking
- **Notifications**: Real-time user engagement system

### API Endpoints
- **RESTful Design**: 50+ endpoints following REST conventions
- **Authentication**: JWT-based authentication with Supabase integration
- **Validation**: Comprehensive request/response validation
- **Error Handling**: Structured error responses with appropriate HTTP status codes
- **Pagination**: Efficient data pagination for large datasets

### Business Logic
- **Stamp Collection**: Secure NFC-based stamp collection with validation
- **Redemption Logic**: Multi-point redemption system with position tracking
- **Progress Tracking**: Real-time stamp collection progress monitoring
- **Notification System**: Automated engagement notifications
- **Geolocation Queries**: Efficient location-based business discovery

## Development Practices

### Code Organization
- **Clean Architecture**: Separation of concerns with repository, service, and handler layers
- **Dependency Injection**: Interface-based dependency management
- **Error Handling**: Centralized error management with custom error types
- **Logging**: Structured logging with context propagation
- **Testing**: Unit and integration test coverage

### DevOps & Deployment
- **Containerization**: Docker support for consistent deployment
- **Database Migrations**: Automated schema management with Goose
- **API Documentation**: Auto-generated OpenAPI documentation
- **Code Quality**: golangci-lint for code quality enforcement
- **Environment Management**: Multi-environment configuration support

## Technical Achievements
- **Scalable Architecture**: Designed for horizontal scaling with stateless services
- **Performance Optimization**: Efficient database queries with proper indexing
- **Security**: JWT authentication, input validation, and secure NFC handling
- **Developer Experience**: Auto-generated API client code and comprehensive documentation
- **Geospatial Features**: PostGIS integration for location-based services
- **Asynchronous Processing**: Background notification creation and event tracking

## Business Impact
- **Digital Transformation**: Enables businesses to modernize their loyalty programs
- **Customer Engagement**: Automated notifications and progress tracking increase customer retention
- **Operational Efficiency**: Automated stamp collection reduces manual processes
- **Data Insights**: Comprehensive tracking provides valuable customer behavior analytics
- **Scalability**: Cloud-native architecture supports business growth

## Technologies & Tools
- **Backend**: Go, Chi, SQLx, PostgreSQL, PostGIS
- **Authentication**: Supabase Auth, JWT
- **API**: OpenAPI 3.0, oapi-codegen
- **Database**: PostgreSQL, Goose migrations
- **Development**: Docker, golangci-lint, Insomnia (API testing)
- **Documentation**: Swagger, Redoc
- **Infrastructure**: Docker Compose, environment-based configuration 


---

**Last Updated**: July 2025