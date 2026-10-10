# Employee Management System

## Student Information

- **Full Name:** Esraa Ahmed Mahmoud
- **Section:** S4
- **Student ID:** 2302006

## Project Description

The **Employee Management System** is an enterprise-oriented Java software designed to model company hierarchies, departmental organization, and multi-tier compensation workflows. Built from the ground up on core Object-Oriented Programming (OOP) paradigms, the application provides an extensible and cleanly partitioned codebase reflecting corporate staff administration.

A foundational abstract class, `Employee`, acts as the unified contract across all personnel categories. It centralizes baseline employee characteristics and mandates custom earnings calculations in respective child classes, demonstrating the effective use of abstraction, class inheritance, and polymorphic method execution to minimize redundant logic and accommodate evolving business requirements.

### Key Features

- **Staff Profile Tracking:** Captures essential worker records including unique IDs, full names, gender identity, employment start date, contact channels, and affiliated department.
- **Support for Diverse Roles:** Accommodates distinct employment arrangements: salaried staff, hourly wage earners, and commission-based personnel.
- **Flexible Payroll Processing:** Computes net compensation dynamically based on employment criteria—incorporating fixed monthly allowances with bonuses, tracked working hours with overtime rates, or targeted sales commission tiers.
- **Departmental Hierarchy:** Groups personnel under designated departments with support for assigning supervising unit managers.
- **Search Capabilities:** Enables looking up staff members by identifier (ID) or name.
- **Input Validation & Safety:** Integrates strict input checks and null-safety constraints across constructors and setters to maintain application state integrity and eliminate runtime crashes.
- **Defensive Encapsulation:** Implements defensive copying for mutable employee datasets to protect internal collections against unintended side effects.

### Object-Oriented Programming Concepts

- **Abstraction:** The base `Employee` class provides shared functionality and establishes the abstract contract for `calculateSalary()`, which concrete subclasses must satisfy.
- **Inheritance:** `MonthlyEmployee`, `HourlyEmployee`, and `CommissionEmployee` inherit from `Employee`, reusing common attributes while defining their specialized business logic.
- **Polymorphism:** Enables handling collections of diverse employee instances uniformly via base-type references while executing subclass-specific salary algorithms dynamically.
- **Encapsulation:** Secures class internals using private fields, exposing them strictly through controlled accessor and mutator methods.
- **Aggregation & Association:** Models relationships between departments and staff, including dedicated manager associations within the `Department` model.
- **Type Safety via Enums:** Standardizes demographic classification using a typed `Gender` enum to restrict invalid data entries.
- **Defensive Design:** Guards data validity using robust field preconditions, null checks, and isolated data collections.

### Project Goals

The objective of this project is to showcase the practical application of object-oriented principles in solving typical enterprise problems. It prioritizes clean code structure, separation of concerns, high maintainability, and seamless extensibility for introducing additional roles or management features in future releases.

## Technologies Used

- **Programming Language:** Java
- **Development Environment:** IntelliJ IDEA
- **Core Concepts:** OOP (Abstraction, Encapsulation, Inheritance, Polymorphism), Java Collections, Enums, Defensive Programming

## Project Structure

```text
EmployeeManagementSystem/
├── src/
│   ├── Main.java
│   ├── model/
│   │   ├── Employee.java
│   │   ├── CommissionEmployee.java
│   │   ├── MonthlyEmployee.java
│   │   ├── HourlyEmployee.java
│   │   ├── Department.java
│   │   └── Gender.java
│   └── test/
│       └── MainTest.java
└── README.md
```

**How to Run the Project

1.Verify that Java Development Kit (JDK 17 or later recommended) is installed on your machine.

2.Clone or extract the project repository locally.

3.Launch IntelliJ IDEA and open the project directory.

4.Set the Project SDK under Project Settings to your installed JDK version.

5.Navigate through the directory tree to src/test/MainTest.java.

6.Execute the main() method to run the demonstration suite with sample department and personnel data.

**Note: Ensure that your IDE detects the src directory as a Source Root and that build configurations point to MainTest.java before running.

## Repository

[https://github.com/EsraaAhmed886/EmployeeManagementSystem](https://github.com/EsraaAhmed886/EmployeeManagementSystem)
