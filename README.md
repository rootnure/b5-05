# Database Essentials and Relational Model

## Data, Database and Information
- Data is facts that can be recorded and/or stored
    - Data is the core of the digital world
- Database is a storage to store data (a computer)
- Information is processed and organized data that provides meaningful context

## DBMS and Why DBMS?
- DBMS --> Database Management System
    - A piece of software to manage data
- Why DBMS?
    - Manage data in a structured way
    - Reduce/Remove redundancy and maintain consistency
    - Security and access management
- SQL --> Structured Query Language

## Different Types of Database Model
- Hierarchical
- Network
- Relational (i.e. MySQL, PostgreSQL)
- Document (i.e. MongoDB)
- Key value (i.e. Radis)

## Anatomy of a Table/Relation (What a DBMS Table can have)
- Entity --> Name of the table or which type of data will be stored in the table in RDBMS
- Column / Attribute --> Which data will be stored.
- Constraint / Domain --> What type of data must be stored in the column
- Degree --> Collection of column
- Rows / Records / Tuples --> Refer to each row of a table
- Cardinality → Collection of rows

## Key and Type of Keys in RDBMS
- Key --> A field or combination of fields that uniquely identifies a record in a table
- Types of keys
    - Super key --> Attribute or set of attributes by which identify a record uniquely
    - Candidate key --> Super key whose proper subset is not a super key
        - Which set of key doesn’t give any more super key after breaking in subsets
    - Primary key --> That doesn’t change, not null and unique
        - Any one of the candidate key that uniquely identify a record
    - Alternate key --> Candidate keys that aren’t chosen as primary key
    - Composite key --> Set of more than one attribute that uniquely identify a record
    - Foreign key --> A key in a table that exists as a primary key in another table
        - Make connections between multiple tables

## Database Design
- SDLC --> Software Development Life Cycle
    - Planning --> What need to build
    - Analysis --> Can it be build, Can it be build in budged, Capability to build
    - System Design --> Build structure of the system
    - Building --> Coding Part
    - Testing --> Is it ok, Meet the expectation
    - Deployment --> Release the final product
- Database Design is a part of System Design
- Purpose of DB Design → Structured organization for efficient DB management and retrieval
- Techniques to design DB
    - Top-down --> System build from a2z
    - Bottom-up --> Build/Reshape from an existing system
    - Hybrid --> Mix of Top-down and Bottom-up
- ER Diagram --> Entity-Relationship Diagram
    - Visual representation used in DB design to illustrate the relationships between entities
- Steps of Top-down technique
    - Step-1: Determining Entities
    - Step-2: Determining Attributes for each Entities
    - Step-3: Relationships among Entities
- Characteristics of Entity (Table)
    - Can be Place, Person, or thing
    - Have some Properties or Attribute
    - Must have Unique Identifier (Primary Key)
    - Should contain more than one instance of data
- ER Diagram Symbols
    - Entity → Rectangle (▭)
    - Attribute → Oval (⬭)
    - Relationship → Diamond (◇)
    - Connection → Line ( — )
    - Primary Key → Attribute name with underline ( <u>ID</u> )
- Cardinality
    - One-to-One (1:1) → One person has one passport
    - One-to-Many (1:N) → One department has many students
    - Many-to-One (N:1) → Many employee works in one company
    - Many-to-Many (N:N) → One student can take many courses and one course has many students
    - Optional One-to-One (0..1:0..1) → A student may or may not taken any course or a course may or may not taken by any student
    - Optional One-to-Many (0..1:N) → A student may or may not taken any course but must be a student of an academy

## Online ER Diagram
- Lucidechart