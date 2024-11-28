# Requirements Analysis

This is a summary of the training course of the Requirements Analysis

 - Module Focus:

    - Business Analysis
    - Requirements Analysis


## Business Analysis:

    - Understand and describe a company's processes.
    - Example: Life cycle of entities (e.g.: order or book status).

## Requirements Analysis:

    - Specify the system's functionalities.
    - Example: Use cases (user interaction with the system).

### Process to build a software:
<div align="center">
  <img src="resources/image01.jpg">
</div>

#### The software development process involves disciplines and subprocesses, such as analysis, design, construction and validation.
- Analysis: Describes the problem.
- Design: Describes the solution.
- Construction: Implements the solution.
- Certification: Tests and validates the solution before delivery.
- The waterfall model follows a linear sequence, where each step is completed before moving on to the next.
- The waterfall model is best suited for areas such as civil engineering, but is not ideal for software development, which is more dynamic and cyclical.

<div align="center">
  <img src="resources/image05.jpg">
</div>

- The unified process is a framework created by Booch, Rumbaugh and Jacobson, which organizes the disciplines in an iterative and incremental manner.
- The unified process divides development into phases: initiation, elaboration, construction and transition.
- The disciplines (business modeling, requirements, analysis, design, implementation, testing, etc.) are applied in different intensities throughout these phases.
- The unified process is iterative and incremental, meaning that disciplines are applied repeatedly in cycles, with continuous improvement.
- Variants of the unified process include the Rational Unified Process (RUP), OpenUP, and Agile Unified Process (AUP).
- Analysis is a subprocess that describes the problem and is part of an incremental process in software development.

<div align="center">
  <img src="resources/image06.jpg">
</div>

- Comparison with Building Construction:

   - Stages: Analysis (understanding the problem), Design (solution design), Construction (implementation), Homologation (validation).
<div align="center">
  <img src="resources/image02.jpg">
</div>

## Artifacts in Business Analysis:
- Business process specification document.
- Entity life cycle.

## Artifacts in Systems Analysis:

<div align="center">
  <img src="resources/image04.jpg">
</div>

### Requirements Analysis:
- Overview of the system (free document).
- Overview of use cases (diagram).
- Specification of use cases (structured document).

### Domain Analysis:
- Conceptual model (data model at the analysis level).

## Difference between Artifact and Tool:
- Artifact: what you want to specify (e.g. business process).
- Tool: means used to specify (e.g. UML activity diagram).

### Examples of Tools:

- Activity diagram (UML) to specify the flow of actions of the business process.
- State machine diagram (UML) for the life cycle of entities.
- Use case diagram (UML) for an overview of use cases.
- Class diagram (UML) for the conceptual model.

## Free and Structured Documents:
- System overview: free document.
- Use case specification: structured document.

## Importance of Differentiating Artifact and Tool:
- The artifact is the final product (e.g., business process).
- The tool is just a means to create the artifact (e.g., activity diagram).

<div align="center">
  <img src="resources/image03.jpg">
</div>

## Definition of Information System: 
- Organizational system used to collect, store and disseminate data.
- Used by companies and organizations to automate business processes.

## Characteristics of Information Systems: 
- Database with business information.
- Forms, reports and process automation (e.g.: purchases, inventory, employees).

## Information Systems Analysis Process: 
- Focused on systems for companies and organizations.
- Main subprocesses: 
    - Business Analysis: Understanding and describing the business, its rules and processes.
    - Systems Analysis: Understanding the needs and requirements to build the system.

<div align="center">
  <img src="resources/image07.jpg">
</div>

## Subdivisions of Systems Analysis:
- Requirements Analysis: Identify what the system needs to do.
- Domain Analysis: Understand the context and environment of the system.

## Objective of Information Systems:
- Automate parts of business processes, making them more efficient.
- Example: Automate calculations and payroll generation in the financial sector.

## Importance of Business Analysis:
- Understanding the business is a prerequisite for specifying an appropriate system.
- Although it is not a systems analysis, business analysis is essential to the process.

<div align="center">
  <img src="resources/image08.jpg">
</div>

# **Requirements Overview**

## **Definition of Requirements**
- A requirement is a condition or characteristic that the system must meet.
- The classification of requirements varies depending on authors and schools of thought.

<div align="center">
  <img src="resources/image09.jpg">
</div>

## **Types of Requirements**

### 1. **Functional Requirements**
- Involve data manipulation (e.g., database operations, queries, saving, etc.).
- **Subcategories**:
    - **With User Interaction**:
        - **Use Cases**:
            - **CRUD**: Create, Retrieve, Update, Delete (registration screens).
            - **Reports**: Generate listings or reports based on input arguments.
            - **Business Processes**: Automation or semi-automation of business processes.
    - **Without User Interaction**:
        - **Batch Processing**: Scheduled tasks (e.g., nightly jobs).
        - **System Integrations**: Data manipulation and information exchange between systems.
        - **Internal Processing**: Internal operations without user interaction.

### 2. **Non-Functional Requirements**
- Do not involve data transformations.
- Also referred to as "quality requirements."
- **Examples**:
    - **Usability**: Intelligibility, ease of use.
    - **Reliability**: Fault tolerance (e.g., resuming processing after an internet outage).
- **Classifications**:
    - **Forbes Mais**.
    - **ISO 9126** (internal and external quality).
- **Observations**:
    - Classifications are not mutually exclusive (a requirement can belong to more than one category).
    - Requirements should be organized into topics in the document.

<div align="center">
  <img src="resources/image10.jpg">
</div>

## **Final Considerations**
- Classifications serve as guidance and help organize the requirements document.

# **Understanding Use Scenarios and Use Cases**

## **Basic Concepts**
- **System Requirements**:
    - Divided into **functional** and **non-functional** requirements.
    - Use cases are part of **functional requirements**.
- **Usage**:
    - Interaction between **actors** and the **system**.
- **System Actors**:
    - Users who interact with the system (e.g., anonymous user, client, administrator, operator).
    - Interaction = **exchange of information** (inputs and outputs).

## **Use Scenario**
- **Definition**:
    - A **linear sequence** of interactions between actors and the system.
    - Does not include branches, conditions, or loops (e.g., "if", "else").
- **Example: Use Scenario "Sell Book"**:
    1. **Input**: User provides their identification (e.g., login).
    2. **Output**: System displays available books (title, cover, price).
    3. **Input**: Client selects the books they want to purchase.
    4. **Output**: System informs the total value and presents registered address options.
    5. **Input**: Client selects the delivery address.
    6. **Output**: System informs the shipping cost, total amount, and list of registered credit cards.
    7. **Input**: Client selects a credit card.
    8. **Output**: System sends the card details and purchase value to the payment processor.
    9. **Input**: Payment processor provides an authorization code.
    10. **Output**: System informs the delivery time.

## **Actors in the Scenario**
- **Anonymous User**: Before identification.
- **Client**: After identification.
- **Payment Processor**: Interacts with the system to process the payment.

## **Differentiation**
- **Use Scenario**:
    - A **linear sequence** of steps.
    - Does not include branches or error handling.
- **Use Case**:
    - Includes alternative scenarios, such as registering a new address or handling errors (to be covered later).

## **Conclusion**
- A **use scenario** is a **linear sequence of interactions** between actors and the system.
- **Use cases** are broader and include alternative scenarios.