# Lab 2: Local Microservice with Carbon UI

## Overview

This lab demonstrates how to use Bob to convert an ESQL module into a complete microservice architecture with a modern web interface. Bob will generate a REST API microservice with Swagger UI documentation and a Carbon Design System-based user interface, all configured for local deployment without any cloud or Docker dependencies.

**What You'll Build:**
- Python Flask REST API microservice
- Swagger UI for API documentation and testing
- Carbon Design System-based web interface
- Local deployment configuration for both applications

**Duration:** 60-90 minutes

**Difficulty:** Intermediate

---

## Prompt for Bob

Copy and paste the following prompt into Bob AI Assistant:

```
I would like to convert the WeatherServiceModule.esql to a MicroService and aslo include Swagger UI to the microservice I would also like to create and deploy a carbon based User Interface and deploy that application locally without any cloud or docker dependencies

Use the name "WeatherMicroservice" for the microservice

Use the name "WeatherLookup" for the UI application
```

---

## Summary

Congratulations! After Bob completes the generation, you will have:

### REST API Microservice
- **Flask Application**: Production-ready REST API with:
  - Weather lookup endpoints
  - Error handling and validation
  - CORS configuration for local development
  - Logging and monitoring hooks
  
- **Swagger UI Integration**: Interactive API documentation at `/swagger`
  - Test endpoints directly in browser
  - View request/response schemas
  - API versioning support

### Carbon Design System UI
- **Modern Web Interface**: Enterprise-grade UI featuring:
  - Carbon Design System components
  - Responsive layout
  - Accessible design patterns
  - Professional styling
  
- **Frontend Logic**: Complete JavaScript application with:
  - API integration
  - Form handling
  - Error display
  - Result formatting

### Local Deployment
- **No Cloud Dependencies**: Everything runs locally
  - Python virtual environment setup
  - Local web server for UI
  - Port configuration (5000 for API, 8000 for UI)
  - Simple start/stop scripts

### Documentation
- **README files**: Complete setup and usage instructions for both applications
- **API Documentation**: Swagger/OpenAPI specification
- **Testing Guide**: How to test the integration

### 🎯 Key Learnings
- ESQL to REST API conversion patterns
- Microservice architecture principles
- Swagger/OpenAPI documentation
- Carbon Design System implementation
- Local development workflows
- Frontend-backend integration

### 📦 Ready to Run
The generated applications can be started immediately:
1. Install Python dependencies for microservice
2. Start the Flask API server
3. Start the UI web server
4. Access Swagger UI and test endpoints
5. Use the Carbon UI to interact with the API

---

**Next Lab:** [Lab 3: ACE Containerization Strategy](Lab3-ACE-Containerization-Strategy.md)
