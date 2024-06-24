# 先占个坑，填不填随缘

# Framework Overview
Design2Code, will aim to bridge the gap between system design and implementation. It will focus on transforming high-level design models (DFDs and ERDs and others) directly into executable code and application structures. 
> Include F/E-web (B/E - node)

# Core Components
Model Interpreter:
   DFD Interpreter: Converts Data Flow Diagrams into service workflows: mapping processes to functions(microservices), data stores to Global StateStore (databases), and data flows to Sequence ( message queues).
   ERD Interpreter: Translates Entity-Relationship Diagrams into abstract entity ( database schemas and ORM models).
   > Intersection parts: DFD flow executing - (ECMA based)

   > F/E :  UI Entity Binding / Event->Store Binding / BOM Binding

   > B/E :  Database binding / NodeApi Binding



# Configuration Interpreter then Raw Code Generator :

1. Backend Code Generator: Generates backend code (e.g., RESTful APIs, microservices) based on the interpreted models.
2. Database Schema Generator: Creates database schemas and migration scripts from ERDs.
3. Frontend Code Generator: Optionally generates frontend code based on DFDs to create forms and interfaces corresponding to the data flows.
  > web-component base material + es6 modules, drop old browser supports

# Configuration Management:

Allows developers to customize and extend the generated code through configuration files, ensuring flexibility and adaptability.


# Integration Layer:

Integrates with existing development tools and CI/CD pipelines to facilitate smooth deployment and testing.
Supports popular frameworks and libraries (developped web-components, should when use interpreter will use vue as first one, after code generator drop framework and use original js+html+css)

# Validation and Testing:

Validates the generated code against the original models to ensure consistency.
Includes automated testing scripts to verify functionality.

# Key Features
Declarative Configuration: Define complex behaviors and integrations through simple configurations.
Extensibility: Plugin architecture to support additional functionalities and third-party integrations.
User-Friendly Interface: Web-based interface for model designing, code generation, and configuration management.
Real-Time Collaboration: Support for collaborative modeling and code generation, facilitating teamwork.
Documentation Generation: Automatically generate technical documentation from models and configurations.


# Example Workflow
## Design Phase:

Use a graphical tool within Design2Code to create DFDs and ERDs.
Define processes, data flows, and entity relationships visually.


## Code Generation Phase:

The Model Interpreter reads the DFDs and ERDs.
The Code Generator produces backend services, database schemas, and optionally, frontend components.

## Integration and Deployment:

  Integrate generated code into existing repositories.
Deploy using standard CI/CD pipelines.

## Validation and Testing:

Validate the code against the models.
  Run automated tests to ensure everything works as expected.
