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

### JMS Message Structure
- **Standard JMS Headers**:
  - JMSMessageClass: jms_text
  - JMSDestination: queue:///JMS.OUTPUT.QUEUE
  - JMSDeliveryMode: 2 (PERSISTENT)
  - JMSPriority: 4
  - JMSCorrelationID: Preserved from MQMD

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

**Next Lab:** [Lab 5: DFDL Schema Creation](Lab5-DFDL-Schema-Creation.md)
