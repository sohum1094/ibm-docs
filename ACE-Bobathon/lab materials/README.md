# IBM App Connect Enterprise (ACE) Labs

## Overview

This folder contains 6 comprehensive hands-on labs for building IBM App Connect Enterprise solutions using Bob AI Assistant. Each lab is designed to be completed independently with step-by-step instructions and copy-paste prompts.

## Lab Series

### Lab 1: XML to JSON Transformation
**File:** `Lab1-XML-to-JSON-Transformation.md`  
**Duration:** 30-45 minutes  
**Difficulty:** Beginner

Create an ESQL module that performs generic XML to JSON transformation.

**What You'll Learn:**
- ESQL programming
- XML parsing (XMLNSC domain)
- JSON generation
- Message flow design

**Prompt:**
```
Create an ESQL module for App Connect Enterprise that performs a generic XML to JSON transformation...
```

---

### Lab 2: Local Microservice with Carbon UI
**File:** `Lab2-Microservice-with-Carbon-UI.md`  
**Duration:** 60-90 minutes  
**Difficulty:** Intermediate

Convert ESQL to a REST API microservice with Swagger UI and create a Carbon Design System-based user interface.

**What You'll Learn:**
- Microservice architecture
- REST API development
- Swagger/OpenAPI documentation
- Carbon Design System
- Local deployment

**Prompt:**
```
I would like to convert an ESQL module to a microservice with Swagger UI and Carbon-based UI...
```

---

### Lab 3: ACE Containerization Strategy
**File:** `Lab3-ACE-Containerization-Strategy.md`  
**Duration:** 45-60 minutes  
**Difficulty:** Advanced

Create a comprehensive plan for moving ACE integrations to containers.

**What You'll Learn:**
- Container architecture
- Configuration management
- Deployment strategies
- Monitoring and observability
- Migration planning

**Prompt:**
```
Create a comprehensive guide for moving App Connect Enterprise integrations to containers...
```

---

### Lab 4: MQ XML to JMS Transformation
**File:** `Lab4-MQ-XML-to-JMS-Transformation.md`  
**Duration:** 45-60 minutes  
**Difficulty:** Intermediate

Build a message flow using MQ Input node (XML domain) and MQ Output node (JMS domain).

**What You'll Learn:**
- MQ Input/Output nodes
- Domain transformations
- JMS message structure
- Queue-based integration
- Correlation ID handling

**Prompt:**
```
Create an App Connect message flow that uses the MQ input node in the XML domain and an MQ output node in the JMS domain...
```

---

### Lab 5: DFDL Schema Creation
**File:** `Lab5-DFDL-Schema-Creation.md`  
**Duration:** 30-45 minutes  
**Difficulty:** Intermediate

Create a DFDL schema for parsing comma-separated data.

**What You'll Learn:**
- DFDL schema design
- CSV parsing
- Data modeling
- Schema validation
- DFDL annotations

**Prompt:**
```
Create a DFDL schema for App Connect Enterprise that parses comma-separated data...
```

---

### Lab 6: DFDL to JSON Message Flow
**File:** `Lab6-DFDL-to-JSON-Message-Flow.md`  
**Duration:** 60-75 minutes  
**Difficulty:** Advanced

Create a complete message flow that receives DFDL messages from MQ, transforms to JSON, and sends to output queue.

**What You'll Learn:**
- DFDL parsing in message flows
- MQ integration
- DFDL to JSON transformation
- End-to-end integration
- Performance testing

**Prompt:**
```
Create a message flow that receives DFDL-formatted messages from MQ, transforms them to JSON, and sends to an output queue...
```

---

## Prerequisites

### Software Requirements
- IBM App Connect Enterprise Toolkit v11.0 or higher
- IBM MQ v9.0 or higher (for MQ-related labs)
- Python 3.7+ (for Lab 2)
- Access to Bob AI Assistant

### Knowledge Requirements
- Basic understanding of ACE concepts
- Familiarity with message flows
- Basic ESQL knowledge
- Understanding of MQ (for relevant labs)

---

## How to Use These Labs

### Step 1: Choose Your Lab
Select a lab based on your learning objectives and skill level. Labs can be completed in any order, though following the sequence is recommended.

### Step 2: Read the Lab Guide
Open the lab markdown file and read through the overview, objectives, and prerequisites.

### Step 3: Copy the Prompt
Each lab includes an optimized prompt in a code block. Copy this prompt exactly as shown.

### Step 4: Submit to Bob
Paste the prompt into Bob AI Assistant and wait for the artifacts to be generated.

### Step 5: Follow the Steps
Work through the lab steps sequentially:
- Verify generated artifacts
- Import into ACE Toolkit
- Deploy and test
- Review documentation

### Step 6: Complete the Checklist
Each lab includes a completion checklist. Mark items as you complete them.

---

## Lab Progression Path

### Beginner Path
1. **Lab 1:** XML to JSON Transformation
2. **Lab 5:** DFDL Schema Creation
3. **Lab 4:** MQ XML to JMS Transformation

### Intermediate Path
1. **Lab 1:** XML to JSON Transformation
2. **Lab 4:** MQ XML to JMS Transformation
3. **Lab 2:** Local Microservice with Carbon UI
4. **Lab 6:** DFDL to JSON Message Flow

### Advanced Path
Complete all labs in sequence (1-6)

---

## Expected Outcomes

After completing all labs, you will be able to:

✅ Create ESQL transformations  
✅ Design message flows  
✅ Work with multiple domains (XML, JSON, JMS, DFDL)  
✅ Integrate with MQ  
✅ Build microservices  
✅ Create modern UIs  
✅ Plan containerization strategies  
✅ Deploy and test ACE solutions  
✅ Handle errors and monitor flows  
✅ Optimize performance  

---

## Lab Artifacts

Each lab generates a complete project structure:

```
[project-name]/
├── Implementation/ or implementation-details/
│   ├── *.msgflow          # Message flow
│   └── *.esql             # ESQL modules
├── test-cases/
│   ├── sample-*.xml/csv   # Test data
│   └── TEST_CASES.md      # Test documentation
├── project.json           # Project configuration
├── README.md              # Project documentation
├── DEPLOYMENT.md          # Deployment guide
└── TESTING_GUIDE.md       # Testing procedures
```

---

## Tips for Success

### 1. Read Before You Start
Review the entire lab guide before beginning to understand the flow and requirements.

### 2. Use Exact Prompts
Copy the prompts exactly as shown for best results with Bob.

### 3. Verify Each Step
Don't skip verification steps. They ensure artifacts are generated correctly.

### 4. Take Notes
Document your learnings, issues encountered, and solutions found.

### 5. Experiment
After completing a lab, try modifying the solution to deepen your understanding.

### 6. Ask Questions
If something isn't clear, ask Bob for clarification or additional details.

---

## Troubleshooting

### Issue: Bob Doesn't Generate All Files

**Solution:**
- Ensure you copied the complete prompt
- Check for any special characters that might have been altered
- Try breaking the prompt into smaller parts
- Ask Bob to generate missing files specifically

### Issue: Import Fails in ACE Toolkit

**Solution:**
- Verify folder structure matches expected layout
- Check file permissions
- Ensure ACE Toolkit version compatibility
- Try importing individual files

### Issue: Deployment Errors

**Solution:**
- Review deployment guide in each project
- Check integration server logs
- Verify MQ connections (for MQ labs)
- Ensure all dependencies are met

---

## Additional Resources

### IBM Documentation
- [ACE Knowledge Center](https://www.ibm.com/docs/en/app-connect/12.0)
- [ESQL Reference](https://www.ibm.com/docs/en/app-connect/12.0?topic=language-esql-reference)
- [Message Flow Nodes](https://www.ibm.com/docs/en/app-connect/12.0?topic=nodes-message-flow-node-reference)

### Learning Resources
- [ACE Tutorials](https://www.ibm.com/docs/en/app-connect/12.0?topic=tutorials)
- [DFDL Specification](https://www.ogf.org/ogf/doku.php/standards/dfdl/dfdl)
- [IBM MQ Documentation](https://www.ibm.com/docs/en/ibm-mq/9.3)

---

## Support

For questions or issues:
1. Review the lab's troubleshooting section
2. Check the generated README.md in each project
3. Consult ACE Knowledge Center
4. Ask Bob for clarification or help

---

## Contributing

If you find issues or have suggestions for improvements:
1. Document the issue clearly
2. Provide steps to reproduce
3. Suggest potential solutions
4. Share with your team

---

## Version History

- **1.0.0** (2026-04-09): Initial release
  - 6 complete labs
  - Optimized prompts for Bob
  - Comprehensive step-by-step instructions
  - Troubleshooting guides
  - Completion checklists

---

## License

Apache License 2.0

---

## Quick Start

Ready to begin? Start with **Lab 1: XML to JSON Transformation**!

```bash
# Open the first lab
cat Lab1-XML-to-JSON-Transformation.md
```

**Happy Learning!** 🚀