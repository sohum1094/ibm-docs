# Lab 5: DFDL Schema Creation

## Overview

This lab demonstrates how to use Bob AI Assistant to create a DFDL (Data Format Description Language) schema for parsing comma-separated data in IBM App Connect Enterprise. Bob will generate a complete DFDL schema that can parse CSV files with proper field definitions, validation rules, and comprehensive documentation.

**What You'll Build:**
- DFDL schema for CSV parsing
- Sample CSV data files
- Schema documentation
- Validation examples

**Duration:** 30-45 minutes

**Difficulty:** Intermediate

---

## Prompt for Bob

Copy and paste the following prompt into Bob AI Assistant:

```
Create a DFDL schema for App Connect Enterprise that parses comma-separated data.

Sample data format:
name,title,phone,email

Requirements:
- Define DFDL schema for CSV format
- Support header row
- Handle quoted fields
- Support multiple records
- Include validation rules
- Add comprehensive annotations

Schema specifications:
- Field separator: comma (,)
- Text encoding: UTF-8
- Line ending: CRLF or LF
- Quote character: double quote (")
- Escape character: backslash (\)

Create the schema in a folder named dfdl-to-json-transformation.

Include:
1. DFDL schema file (.xsd)
2. Sample CSV data file
3. Documentation explaining the schema
4. Validation examples
5. Usage instructions
```

---

## What Bob Will Create

Bob will generate a complete DFDL schema project:

```
dfdl-to-json-transformation/
├── Implementation/
│   └── EmployeeData.xsd                 # DFDL schema
├── test-cases/
│   ├── sample-employee-data.csv         # Sample CSV data
│   └── expected-output.json             # Expected parsed result
├── project.json                          # Project configuration
└── README.md                             # Schema documentation
```

---

## Summary

After Bob completes the generation, you will have:

### ✅ DFDL Schema
- **CSV Parser Definition**: Complete XSD schema with DFDL annotations
  - Field definitions (name, title, phone, email)
  - Delimiter configuration (comma separator)
  - Line terminator handling
  - Character encoding (UTF-8)
  
- **Format Properties**:
  - separator: ","
  - terminator: "%NL;" (newline)
  - encoding: "UTF-8"
  - lengthKind: "delimited"
  - textTrimKind: "none"

### ✅ Data Model
- **Employee Record Structure**:
  - name: String field
  - title: String field
  - phone: String field with pattern validation
  - email: String field with pattern validation
  
- **Validation Rules**:
  - Email format validation
  - Phone number format validation
  - Required field checks

### ✅ Sample Data
- **CSV Test File**: Sample employee data with:
  - Header row
  - Multiple data records
  - Various field values
  - Edge cases

### ✅ Documentation
- **README**: Schema explanation and usage
- **Annotations**: Inline documentation in schema
- **Examples**: How to use the schema in message flows

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

**Next Lab:** [Lab 6: DFDL to JSON Message Flow](Lab6-DFDL-to-JSON-Message-Flow.md)
