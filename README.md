# 🚌 Paris Arrow Transit Database Design

This project delivers a fully normalized **relational database** for **Paris Arrow Transit (PAT)**, a fictional transport company subcontracted by the Olympic Federation to manage the transportation of officials during the Olympic Games.

The database schema was designed through **entity-relationship (ER) data modeling** and implemented in **Oracle Database**. It includes a complete schema script with entities, relationships, constraints, and embedded business rules.

## Project Overview

PAT requires a centralized system to manage:
- A fleet of vehicles and their features
- Drivers with training records, language skills, and security clearance
- National Olympic Committees (NOCs) and their officials
- Booked trips including vehicle assignment, driver, locations, and preferred language
- Training modules with expiry logic and completion tracking
- Multilingual support using ISO 639-1 codes

The schema includes **15 main tables** and **40+ constraints**, embedding key business rules such as:
- Driver suspension status
- Unique vehicle-trip constraints by datetime
- Chef de Mission as a self-referencing official
- Expiring training modules and module count tracking
- Many-to-many support (e.g., driver-language, vehicle-feature)

## Logical ER Diagram

A **logical entity-relationship diagram (ERD)** is included in the repository as `pat_logical.pdf`. It illustrates the structure of the PAT database, including:

- Entities (tables)
- Attributes (columns)
- Primary and foreign keys
- Relationship cardinality

## Technologies Used

- **Database Platform**: Oracle 12c
- **Modeling Tool**: Oracle SQL Developer Data Modeler 23.1
- **Language**: SQL (DDL)

## Authors

Developed by Juan Nathan, Chloe Tan, and Raynen Athirathan of Group 27 for FIT3171 at Monash University Malaysia.










