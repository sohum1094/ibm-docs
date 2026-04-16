# IBM App Connect Enterprise (ACE) - Complete Lab Guide

## Building ACE Solutions with Bob AI Assistant

---

# Lab 1: XML to JSON Transformation

## Overview

This lab demonstrates how to use Bob AI Assistant to create an ESQL module that performs a generic XML to JSON transformation in IBM App Connect Enterprise. Bob will generate a complete, production-ready solution including the ESQL code, message flow, project configuration, comprehensive documentation, deployment guides, and test cases.

**What You'll Build:**
- ESQL transformation module for XML to JSON conversion
- Message flow with HTTP Input and HTTP Reply nodes
- Complete project structure with documentation
- Test cases for various XML structures

---

## Prompt for Bob

Copy and paste the following prompt into Bob AI Assistant:

```
Create an ESQL module for App Connect Enterprise that performs a generic XML to JSON transformation.

Create the technical artifacts for the ESQL module in a separate folder named xml-to-json-transformation.
```

---

## Summary

Congratulations! After completing this lab, you will have created a complete ESQL module for App Connect Enterprise. 

**Transformation Capabilities:**
- Handles simple XML elements and converts them to JSON properties
- Processes nested XML structures maintaining hierarchy
- Converts XML attributes to JSON properties with `@` prefix
- Detects repeated XML elements and creates JSON arrays automatically
- Supports mixed content (elements with both text and child elements)
- Processes XML with namespaces
- Includes comprehensive error handling with detailed error messages

**Deployment Ready:**
The application is ready to be packaged into a BAR file and deployed to an ACE Integration Node. The HTTP endpoint accepts POST requests with XML payloads and returns JSON responses with proper error handling.

### 📦 Ready to Deploy
The generated artifacts are production-ready and can be:
1. Imported into ACE Toolkit
2. Packaged into a BAR file
3. Deployed to an integration server
4. Tested with the provided sample test-case files

---

**Next Lab:** [Lab 2: Local Microservice with Carbon UI](#lab-2-local-microservice-with-carbon-ui)

---

# Lab 2: Local Microservice with Carbon UI

## Overview

This lab demonstrates how to use Bob to convert an ESQL module into a complete microservice architecture with a modern web interface. Bob will generate a REST API microservice with Swagger UI documentation and a Carbon Design System-based user interface, all configured for local deployment without any cloud or Docker dependencies.

**What You'll Build:**
- Python Flask REST API microservice
- Swagger UI for API documentation and testing
- Carbon Design System-based web interface
- Local deployment configuration for both applications

---

## Prompt for Bob

Copy and paste the following prompt into Bob AI Assistant:

```
I would like to convert the WeatherServiceModule.esql to a MicroService and also include Swagger UI to the microservice I would also like to create and deploy a carbon based User Interface and deploy that application locally without any cloud or docker dependencies

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

**Next Lab:** [Lab 3: ACE Containerization Strategy](#lab-3-ace-containerization-strategy)

---

# Lab 3: ACE Containerization Strategy

## Overview

This lab demonstrates how to use Bob AI Assistant to create a comprehensive strategic plan for moving IBM App Connect Enterprise integrations to containers. Bob will generate a detailed guide covering all aspects of containerization including technical considerations, deployment strategies, testing approaches, and operational best practices.

**What You'll Build:**
- Comprehensive containerization strategy document
- Technical architecture guidance
- Migration planning framework
- Best practices and common pitfalls guide

---

## Prompt for Bob

Copy and paste the following prompt into Bob AI Assistant:

```
Create a comprehensive guide for moving App Connect Enterprise integrations to containers. What are the considerations to move an App Connect Enterprise integration to containers?
```

---

## Summary

After completing this lab, you will have a comprehensive containerization strategy guide covering all aspects of moving IBM App Connect Enterprise integrations to containers:

**Strategic Value:**
This guide provides a complete framework for planning and executing ACE containerization projects, from initial assessment through production operations, with platform-specific guidance and proven best practices.

---

**Next Lab:** [Lab 4: MQ XML to JMS Transformation](#lab-4-mq-xml-to-jms-transformation)

---

# Lab 4: MQ XML to JMS Transformation

## Overview

This lab demonstrates how to use Bob to create a message flow that transforms XML messages from an MQ queue to JMS format on another MQ queue. Bob will generate a complete queue-to-queue integration using MQ Input and Output nodes with domain transformation from XMLNSC to JMS.

**What You'll Build:**
- Message flow with MQ Input node (XML domain)
- Message flow with MQ Output node (JMS domain)
- ESQL transformation logic
- Complete MQ configuration and deployment guides

---

## Prompt for Bob

Copy and paste the following prompt into Bob AI Assistant:

```
Create an App Connect message flow that uses the MQ input node in the XML domain and an MQ output node in the JMS domain.

Create all the technical and other artifacts in a separate folder named implementation-details under the xml-to-jms-mq-transformation folder.
```

---

## Summary

After Bob completes the generation, you will have:

### Message Flow Components
- **MQ Input Node**: Configured for XMLNSC domain

- **Compute Node**: ESQL transformation logic
  - Reads XML
  - Converts to JMS message structure
  - Sets JMS headers and properties
  
- **MQ Output Node**: Configured for JMS domain

### Transformation Logic
- **XML to JMS Conversion**: Complete ESQL module featuring:
  - XML serialization to string
  - JMS message structure creation
  - Header mapping (Destination, DeliveryMode, Priority)
  - Correlation ID preservation
  - Custom tracking properties

### 🎯 Key Learnings
- MQ Input/Output node configuration
- Domain transformations (XMLNSC to JMS)
- JMS message structure and properties
- Correlation ID handling
- Queue-based integration patterns
- Error handling with backout queues

### 📦 Ready to Deploy
The generated artifacts can be:
1. Imported into ACE Toolkit
2. Deployed to integration server
3. Tested with MQ commands (amqsput/amqsget)
4. Monitored with MQ and ACE tools

---

**Lab 4 Backup Video**[Lab 4 Video](./assets/videos/lab4backup.mp4)

---

**Next Lab:** [Lab 5: DFDL Schema Creation](#lab-5-dfdl-schema-creation)

---

# Lab 5: DFDL Schema Creation

## Overview

This lab demonstrates how to use Bob AI Assistant to create a DFDL (Data Format Description Language) schema for parsing comma-separated data in IBM App Connect Enterprise. Bob will generate a complete DFDL schema that can parse CSV files with proper field definitions, validation rules, and comprehensive documentation.

**What You'll Build:**
- DFDL schema for CSV parsing
- Sample CSV data files
- Schema documentation
- Validation examples

---

## Prompt for Bob

Copy and paste the following prompt into Bob AI Assistant:

```
Create a DFDL schema for App Connect Enterprise that parses comma-separated data.

Sample data format:
name,title,phone,email
```

---

## Summary

After Bob completes the generation, you will have:

### DFDL Schema
- **CSV Parser Definition**: Complete XSD schema with DFDL annotations
  - Field definitions (name, title, phone, email)
  - Delimiter configuration (comma separator)
  - Line terminator handling
  - Character encoding (UTF-8)

### 🎯 Key Learnings
- DFDL schema structure and syntax
- CSV parsing with DFDL
- Field delimiter configuration
- Data type definitions
- Validation patterns
- Schema reusability

### 📦 Ready to Use
The generated schema can be:
1. Imported into ACE Toolkit
2. Used in message flows with DFDL parser
3. Validated against sample data
4. Extended for additional fields
5. Reused across multiple flows

---

**Next Lab:** [Lab 6: DFDL to JSON Message Flow](#lab-6-dfdl-to-json-message-flow)

---

# Lab 6: DFDL to JSON Message Flow

## Overview

This lab demonstrates how to use IBM Bob to create a complete end-to-end message flow that receives DFDL-formatted CSV messages from an MQ queue, parses them using the DFDL schema from Lab 5, transforms the data to JSON format, and sends the JSON to an output MQ queue. This represents a complete integration solution.

**What You'll Build:**
- Complete message flow with MQ Input and Output nodes
- DFDL parser integration
- DFDL to JSON transformation
- Comprehensive testing and deployment guides

---

## Prompt for Bob

Copy and paste the following prompt into Bob AI Assistant:

```
Create a message flow that receives DFDL-formatted messages from MQ, transforms them to JSON, and sends to an output queue.

Create all the required implementation details and other technical artifacts in a separate folder named Implementation under the dfdl-to-json-transformation project folder.
```

---

## Summary

After Bob completes the generation, you will have:

### Complete Message Flow
- **MQ Input Node**: Receives CSV messages
  - Queue
  - Message Domain: DFDL
  - Message Model
  - Automatic CSV parsing
  
- **Compute Node**: DFDL to JSON transformation
  - Reads parsed DFDL structure
  - Creates JSON array
  - Maps all fields
  - Adds metadata
  
- **MQ Output Node**: Sends JSON messages
  - Queue
  - Message Domain: JSON
  - Formatted output

### Transformation Logic
- **ESQL Module**: Complete transformation featuring:
  - DFDL tree traversal
  - JSON structure creation
  - Array handling for multiple records
  - Field mapping (name, title, phone, email)
  - Error handling
  - Validation

### End-to-End Integration
- **CSV Input**: Comma-separated employee data
- **DFDL Parsing**: Automatic parsing using schema
- **JSON Output**: Structured JSON array
- **Error Handling**: Invalid data routing
- **Monitoring**: Flow statistics and logging

### MQ Configuration
- **Queue Setup**: Complete MQSC commands for:
  - DFDL input queue
  - JSON output queue
  - Error queue
  - Queue permissions

### 🎯 Key Learnings
- DFDL parser integration in message flows
- DFDL to JSON transformation patterns
- End-to-end MQ integration
- Error handling strategies
- Performance testing approaches
- Production deployment practices

### 📦 Ready for Production
The complete solution includes:
1. Production-ready message flow
2. Comprehensive error handling
3. Complete documentation
4. Test cases and procedures
5. Deployment automation
6. Monitoring and logging

---

## Series Complete!

**Congratulations!** You have completed all 6 labs in the IBM App Connect Enterprise series.

### What You've Accomplished:
1. ✅ XML to JSON transformation
2. ✅ Microservice development with Carbon UI
3. ✅ ACE containerization strategy
4. ✅ MQ XML to JMS transformation
5. ✅ DFDL schema creation
6. ✅ DFDL to JSON message flow

### Next Steps:
- Apply these patterns to your own projects
- Explore advanced ACE features
- Build custom integrations
- Share knowledge with your team

**Happy Integrating!** 🚀

---
