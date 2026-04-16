# Lab 1: XML to JSON Transformation

## Overview

This lab demonstrates how to use Bob AI Assistant to create an ESQL module that performs a generic XML to JSON transformation in IBM App Connect Enterprise. Bob will generate a complete, production-ready solution including the ESQL code, message flow, project configuration, comprehensive documentation, deployment guides, and test cases.

**What You'll Build:**
- ESQL transformation module for XML to JSON conversion
- Message flow with HTTP Input and HTTP Reply nodes
- Complete project structure with documentation
- Test cases for various XML structures

**Duration:** 30-45 minutes

**Difficulty:** Beginner

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

**Next Lab:** [Lab 2: Local Microservice with Carbon UI](Lab2-Microservice-with-Carbon-UI.md)