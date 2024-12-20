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

<div align="center">
  <img src="resources/image11.jpg">
</div>

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

<div align="center">
  <img src="resources/image12.jpg">
</div>

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

# **Understanding Use Case Scenarios**

## **Definition of a Use Case**
- A use case is a set of interrelated usage scenarios aimed at a specific objective.
- It includes:
    - **Main Scenario**: The ideal flow where everything works as expected.
    - **Alternative Scenarios**: Different paths or exceptions that may occur.

## **Example of a Use Case**
- **Use Case: Selling a Book**
    - **Main Scenario**: A linear sequence of steps to sell a book.
    - **Alternative Scenarios**: Different paths or exceptions, such as invalid identification.

## **Components of a Use Case**
. **Main Scenario**:
- The ideal sequence of steps.
  . **Exception Scenarios**:
- Handle errors, such as invalid identification.
  . **Variant Scenarios**:
- User options, such as registering a new address.

## **Numbering Alternative Scenarios**
- Alternative scenarios are numbered based on the step in the main scenario that caused the deviation.
- Example:
    - **Exception 1A**: Occurs at step 1 of the main scenario.

## **Data Specificity**
- Each step must detail the required information (e.g., street, number, ZIP code).
- This helps developers create accurate screens and functionalities.

## **Use Case Utility**
. **Design**:
- Guides designers in defining operations and API endpoints.
  . **Implementation**:
- Helps developers ensure all requirements are met.
  . **Testing**:
- Assists analysts in designing tests aligned with the data and flows.

## **Use Case as a Contractual Tool**
- Demonstrates the complexity of the operation.
- Facilitates cost estimation and pricing for clients.

## **Complete Example**
- **Main Scenario**:
    - A detailed sequence of steps.
- **Exception Scenarios**:
    - Example: **Exception 1A** - Invalid identification.
        - Step 1A.1: The system informs the user that the identification is invalid.
        - Step 1A.2: The system requests the user to re-enter their identification.
- **Variant Scenarios**:
    - Example: **Variant 4.1** - Register a new address.
        - Step 4.1.1: The user provides street, number, complement, ZIP code, city, and state.
        - Step 4.1.2: The process returns to step 6.

## **Key Notes**
- Always specify the data required in each step.
- Ensure clarity for developers to implement the correct functionality.

# Documentation: Attributes of a Use Case

This document describes the main attributes of a use case, based on best practices for system modeling.

## Attributes of a Use Case

### 1. **Interactivity**
- A use case must involve **information exchange** between the system and the actors.
- Complementary steps can be included for better understanding, but the main focus should be on the exchange of information.

### 2. **Single Session**
- The use case must occur within a **single session of system use**.
- **Session**: the time interval during which the user is using the system.
- Example: the user starts an operation, performs the necessary actions, and finishes without interruptions.
- Complex operations that require more than one session should be divided into **multiple use cases**.

### 3. **Consistent Result**
- The system must start and finish the use case in a **consistent state**.
- There must be no pending operations or incomplete calculations at the end of the use case.
- Even in case of failure or abortion, the system must remain consistent.

## Examples of Use Cases
- **Making a purchase**: the user selects items, makes the payment, and completes the purchase in a single session.
- **Registering a payment**: the user enters payment details and confirms the operation, leaving the system in a consistent state.

---

## Conclusion

Following these attributes ensures that use cases are well-defined, promoting clarity and consistency in system development.

<div align="center">
  <img src="resources/image13.jpg">
</div>

# Documentation: Use Case Diagram vs. Use Case Detailing

This document explains the key differences between a use case diagram and the detailing of use cases, based on best practices for system modeling.

## Key Differences

### 1. **Use Case Diagram**
- Provides a **high-level overview** of the system.
- Displays the **actors** and the **use cases**.
- Acts as a **panoramic view** of the system's use cases.

### 2. **Use Case Detailing**
- Contains the **true value** of the use case.
- Describes the **steps** and the **information exchanged** between the user and the system.
- Focuses on **best practices** and **techniques** to create effective use cases.

### 3. **Importance of Differentiation**
- It is crucial to understand that the diagram is only a high-level overview, while the detailing provides deeper and more practical insights.

## Next Steps
- Learn how to create use case diagrams to express the system's overall view.
- Study how to effectively detail use cases using best practices and techniques.

---

## Conclusion

Understanding the distinction between use case diagrams and their detailing ensures clarity in system modeling and helps in creating effective use cases.

<div align="center">
  <img src="resources/image14.jpg">
</div>

# Documentation: Overview of Use Case Diagrams

This document provides an overview of use case diagrams, their purpose, and how they are used to represent the use cases of a system.

## Overview of Use Case Diagrams

### 1. **Purpose of the Use Case Diagram**
- The use case diagram is a **graphical tool** used to present a **high-level overview** of the system's use cases.
- It is part of the **UML (Unified Modeling Language)** and is designed to be simple and easy to understand.

### 2. **Key Components**
- **Use Cases**: Represented as **ellipses** with names, typically starting with a **verb**.
- **Actors**: Represented as **stick figures** (users or systems interacting with the use cases).
- **Relationships**: Lines connecting actors to the use cases they interact with.

### 3. **Example: Flight Reservation System**
- Use cases include:
    - Search for flights.
    - Cancel reservation.
    - Register flight.
    - Search for airplanes.
    - Book flight.
    - Perform flight upgrade.
- These use cases represent the main functionalities of the system.

### 4. **Characteristics of Use Case Diagrams**
- **Simplicity**: A straightforward graphical tool that does not require technical expertise to understand.
- **Analysis Specification**: Focused on describing the problem, not on technical implementation.
- **Accessibility**: Designed to be understood by business stakeholders and non-technical users.

### 5. **Purpose in Analysis**
- The use case diagram is used to:
    - Represent the **use cases** (ellipses).
    - Identify the **actors** (stick figures) interacting with the use cases.
    - Show the **relationships** between actors and use cases.

---

## Conclusion

Use case diagrams are a simple yet powerful tool for representing the high-level functionalities of a system. They are accessible to both technical and non-technical stakeholders, making them an essential part of the analysis phase in system design.

<div align="center">
  <img src="resources/image15.jpg">
</div>

# Documentation: Use Case Diagram - Basic Palette Items

This document provides an overview of the basic palette items used in a use case diagram and an example of their application in a flight reservation system.

## Overview of Basic Palette Items

### 1. **Key Elements of the Diagram**
- **Use Case**: Represented by **ellipses**.
- **Actor**: Represented by a **stick figure**.
- **Interaction**: Represented by a **line** connecting actors and use cases.
- **System**: Represented by a **rectangle** that delimits the system or module being specified.

### 2. **Example: Flight Reservation System**
#### Use Cases and Interactions:
- **Search Flights**:
    - **Actors**: User (anonymous), Client, and Agent.
    - **Interaction**: All three actors interact with the "Search Flights" use case.
- **Cancel Reservation**:
    - **Actor**: Client.
    - **Interaction**: Only the client interacts with the "Cancel Reservation" use case.
- **Book Flights**:
    - **Actors**: Client and Agent.
    - **Interaction**: Both interact with the "Book Flights" use case.
- **Register Flights**:
    - **Actor**: Secretary.
    - **Interaction**: Only the secretary interacts with the "Register Flights" use case.

### 3. **Purpose of the Diagram**
- Provide a **high-level overview** of the interactions between actors and use cases.
- Focus on **who interacts with what** in the system.
- Keep it **simple and easy to understand** without delving into details.

---

## Conclusion

The use case diagram is a straightforward tool to visualize the relationships between actors and use cases in a system. By using basic elements such as ellipses, stick figures, lines, and rectangles, it provides a clear and concise representation of the system's functionality.

<div align="center">
  <img src="resources/image16.jpg">
</div>

# Generalization in Use Case Diagrams

## Overview
This document explains the concept of **generalization** in UML use case diagrams, as discussed in the lesson.

## What is Generalization?
Generalization in use case diagrams works similarly to inheritance in object-oriented programming. It allows actors to inherit behaviors and interactions from a more general actor.

### Example:
- **Client is a User**:
  - The client can access everything a user can, plus additional specific functionalities.
- **Agent is a User**:
  - The agent can access everything a user can, plus additional specific functionalities.

## Benefits of Generalization
- **Simplifies the Diagram**:
  - By using generalization, the number of lines in the diagram is reduced.
  - Example:
    - Since both client and agent inherit from the user, they automatically interact with the use cases associated with the user.
    - No need to draw separate lines between client/agent and the use cases (e.g., "Search Flights").

## How to Read Generalization Relationships
- The relationship is read as:
  - **Client is a User**.
  - **Agent is a User**.
- This is similar to the inheritance concept in object-oriented programming.

## Key Takeaways
- Generalization helps to organize and simplify use case diagrams.
- It reduces redundancy by grouping shared behaviors under a general actor.
- The relationship is intuitive and follows the "is-a" principle.

---

**Example Diagram**:
- Actors: User, Client, Agent.
- Use Case: "Search Flights".
- Generalization:
  - Client and Agent inherit from User.
  - No need to draw separate lines between Client/Agent and "Search Flights".

---

Thank you for reading! Feel free to contribute or ask questions.

<div align="center">
  <img src="resources/image17.jpg">
</div>

# Extend Relationship in Use Case Diagrams

## Overview
This document explains the **extend relationship** in UML use case diagrams, as discussed in the lesson.

## What is the Extend Relationship?
The extend relationship is used to indicate that one use case **optionally extends** the functionality of another use case. It is represented by a **dotted arrow** with the label `<<extend>>`.

### Key Characteristics:
- The arrow points **from the extending use case** to the **base use case**.
- The extending use case represents **optional functionality** that occurs in **specific scenarios** of the base use case.

## When to Use the Extend Relationship?
Use the extend relationship when:
- The extending use case is **not always executed** as part of the base use case.
- The functionality it provides is **optional** and depends on specific conditions.

### Example:
- **Base Use Case**: "Reserve Flight".
- **Extending Use Case**: "Upgrade Flight".
- Explanation:
  - A user commonly reserves a flight.
  - Occasionally, the user may choose to upgrade the flight, which is an optional action.
  - The relationship is represented as: `Upgrade Flight` **extends** `Reserve Flight`.

## How to Read the Extend Relationship?
The relationship is read as:
- "`Upgrade Flight` extends the functionality of `Reserve Flight`."

## Scenarios
- There must be scenarios in the base use case where the extending use case is **not executed**.
- In the detailed steps of the base use case, there should be an indication of the possibility to execute the extending use case.

---

## Example Diagram
- **Base Use Case**: Reserve Flight.
- **Extending Use Case**: Upgrade Flight.
- **Relationship**: `Upgrade Flight` extends `Reserve Flight`.

---

## Key Takeaways
- The extend relationship is used to represent **optional functionality** in use case diagrams.
- It simplifies the representation of scenarios where additional actions may or may not occur.
- The relationship is intuitive and helps to clarify optional interactions in the system.

---

Thank you for reading! Feel free to contribute or ask questions.

<div align="center">
  <img src="resources/image18.jpg">
</div>

# Include Relationship in Use Case Diagrams

## Overview
This document explains the **include relationship** in UML use case diagrams, as discussed in the lesson.

## What is the Include Relationship?
The include relationship is used to indicate that one use case **always includes** the execution of another use case during its process. It is represented by a **solid arrow** with the label `<<include>>`.

### Key Characteristics:
- The arrow points **from the base use case** to the **auxiliary use case**.
- The auxiliary use case is **mandatory** and will always be executed as part of the base use case.

## Differences Between Include and Extend
. **Direction of the Arrow**:
- In the include relationship, the arrow **starts from the base use case** and **points to the auxiliary use case**.
- In the extend relationship, the arrow **points to the base use case**.
  . **Obligation**:
- In the include relationship, the auxiliary use case is **mandatory**.
- In the extend relationship, the extending use case is **optional**.

## Example
- **Base Use Case**: "Register Flight".
- **Auxiliary Use Case**: "Search Aircraft".
- **Explanation**:
  - Whenever the secretary executes "Register Flight", they must **always** execute "Search Aircraft" as part of the process.
  - However, "Search Aircraft" can also be executed **independently**, without being tied to "Register Flight".

## How to Read the Include Relationship?
The relationship is read as:
- "`Register Flight` includes the functionality of `Search Aircraft`."

## Why Represent It in the Diagram?
Although "Search Aircraft" is included in "Register Flight", it is also an **independent use case**. For example:
- The secretary can log into the system, search for an aircraft, and exit without registering a flight.

---

## Key Takeaways
- The include relationship is used to represent **mandatory functionality** in use case diagrams.
- It ensures clarity in scenarios where a use case depends on another but also allows for independent execution of the auxiliary use case.
- The relationship helps to simplify and organize the representation of system interactions.

---

Thank you for reading! Feel free to contribute or ask questions.

<div align="center">
  <img src="resources/image19.jpg">
</div>

# Lesson Theme: Detailing System Use Cases

## Definition of Detailing:
- Also known as **use case expansion**.
- Specifies the **steps of interaction** between users and the system.
- Includes:
  - **Main Scenario**: A list of primary steps.
  - **Alternative Scenarios**:
    - **Exceptions**: Error handling.
    - **Variants**: User options (not errors).

<div align="center">
  <img src="resources/image20.jpg">
</div>

### Forms of Description:
. **Textual Structured Description** (Preferred):
- Simple and straightforward.
- Specifies **inputs and outputs** of information.
  . **Tabular Description**:
- One column for the actor and another for the actions performed.
- Details the information exchanged in each step.
  . **Graphical Description**:
- Uses **activity diagrams** (action flow diagrams).
- Can become overloaded with too much information.

### Considerations:
- Specification should be **quick and agile** to save time.
- UML does not define a standard for the textual description of steps.
- Best practices will be covered in future lessons.

<div align="center">
  <img src="resources/image21.jpg">
</div>

# Use Case Documentation Template

This repository provides a basic template for describing use cases. The template includes the main sections and guidelines to ensure clarity and completeness when documenting functional requirements.

## Template Overview

### 1. **Actors and Stakeholders**
- Identify the actors involved in the use case.
- Specify stakeholders, such as departments or other interested parties (e.g., Marketing Department).

### 2. **Preconditions and Postconditions**
- **Preconditions**: Conditions assumed to be true before the use case starts (e.g., operator logged into the system).
- **Postconditions**: Conditions assumed to be true after the use case ends successfully (e.g., book sold).

### 3. **Overview**
- A brief explanation of the use case to help with quick identification and understanding.
- Can be used for cost estimation purposes.

### 4. **Main Success Scenario**
- The most common sequence of steps where everything works as expected without errors.

### 5. **Alternative Scenarios**
- **Variants**: Different options the user can follow.
- **Exceptions**: Error scenarios and how they are handled.

### 6. **Additional Information**
- Include complementary details such as:
  - Screen prototypes.
  - Related requirements or business rules.
  - Mathematical formulas or expressions.
  - Technological variations (e.g., mobile vs. desktop behavior).
  - Open questions (e.g., pending decisions about payment methods like PIX or credit card).
  - Detailed descriptions of data if too extensive to include in the main steps.

## Example Use Case Structure

```markdown
# Use Case: [Use Case Name]

## Overview
A brief description of the use case.

## Actors
- [Actor 1]
- [Actor 2]

## Stakeholders
- [Stakeholder 1]
- [Stakeholder 2]

## Preconditions
- [Precondition 1]
- [Precondition 2]

## Postconditions
- [Postcondition 1]
- [Postcondition 2]

## Main Success Scenario
. [Step 1]
. [Step 2]
. [Step 3]

## Alternative Scenarios
### Variants
- [Variant 1]
- [Variant 2]

### Exceptions
- [Exception 1]
- [Exception 2]

## Additional Information
- [Prototype links, business rules, or other relevant details]

```
<div align="center">
  <img src="resources/image23.jpg">
</div>

<div align="center">
  <img src="resources/image24.jpg">
</div>

<div align="center">
  <img src="resources/image25.jpg">
</div>

