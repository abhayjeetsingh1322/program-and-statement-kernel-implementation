# Program and Statement Kernel Implementation

## Description
This project involves the implementation and testing of kernel components for a **BL compiler**:
1. **ProgramKernel**: Manages BL programs using a `Map<String, Statement>` for context and a `Statement` for the program body.
2. **StatementKernel**: Represents and manipulates BL statements using a `Tree<StatementLabel>` for efficient operations.

This project emphasizes:
- Implementing kernel methods for `Program` and `Statement`.
- Leveraging abstract data types such as `Map` and `Tree` to ensure modularity.
- Writing comprehensive tests for these critical compiler components.

---

## Objectives
1. Implement the `ProgramKernel` interface with operations to manage program names, context, and body.
2. Implement the `StatementKernel` interface with operations to handle complex statement structures.
3. Develop specification-based test plans to thoroughly validate both components.

---

## Features
### 1. ProgramKernel
- **Core Operations**:
  - **`setName`**: Sets the program name.
  - **`name`**: Retrieves the program name.
  - **`newContext`**: Replaces the context with a new map.
  - **`swapContext`**: Swaps the current context with a provided map.
  - **`newBody`**: Replaces the program body with a new statement.
  - **`swapBody`**: Swaps the current body with a provided statement.

### 2. StatementKernel
- **Core Operations**:
  - **Block Manipulation**:
    - `addToBlock`
    - `removeFromBlock`
    - `lengthOfBlock`
  - **Control Structures**:
    - `assembleIfElse` / `disassembleIfElse`
    - `assembleWhile` / `disassembleWhile`
  - **Procedure Call**:
    - `assembleCall` / `disassembleCall`

---

## Technologies Used
- **Java**: For implementing kernel classes and operations.
- **JUnit**: For unit testing and validating kernel components.

---

## How to Run
### Prerequisites
- Java Development Kit (JDK)
- Any Java-compatible IDE or terminal

### Steps
1. Clone the repository:
   ```bash
   git clone [repository URL]
