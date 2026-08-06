# ICT / OL & AL / FREE Tutorial & Study Material

### Made specifically for Sri Lankan OL & AL Students.
#### The above /OL-Tutes/ folder contains the following subjects

1. Number Systems
2. Logic Gates
3. Software Lifecycles
4. General information
5. Database handling
6. Algorithms
7. Word Processing
8. Excel/Calc Spreadsheets
9. Operating Systems
10. Web Designing

## Logic Gates
##### Logic gates are the funadmental components of a Microprocessor or decision making circuit. Think of it as a fundamental electronic building block of digital systems. It performs a basic logical operation on one or more binary inputs (voltages representing 1 or 0) to produce a single binary output. They are the electronic "switches" that make up everything from smartphones to processors

![Logic Gates]( /OL-Tutes/gates-git.jpg )

If you like building logic gates, learn about the BC547 transistor and start off by building AND, OR gates.

## Operating Systems
#### An operating system (OS) is essential system software that manages a computer's hardware and software resources. It acts as a bridge between users, application programs, and physical components like the CPU, memory, and storage. Common examples include Microsoft Windows, Apple macOS, Linux, Android, and iOS.

![Operating System]( /OL-Tutes/os-hw3.jpg )

### Core Functions
- Memory management: Tracks and assigns RAM to active programs safely.
- Process management: Controls how the CPU handles tasks and switches between them.
- File management: Organizes, saves, and protects data on storage drives.
- Device control: Communicates with hardware using specialized drivers.

### Common Types
- Desktop OS: Built for personal computers (Windows, macOS, Linux).
- Mobile OS: Built for smartphones and tablets (Android, iOS).
- Server OS: Built to manage network traffic and enterprise data (Linux, UNIX).

![Example OS]( /OL-Tutes/examples_of_os.webp )

## Database Tables & Relationships
Database relationships are logical connections between different tables. They use special fields called primary keys and foreign keys to link data safely and avoid repeating information.Types of Relationships
- One-to-One (1:1): One row in a table links to only one row in another table. Example: A user and their specific profile details.
- One-to-Many (1:N): One row in a table links to multiple rows in another table. Example: One customer places many orders.
- Many-to-Many (N:N): Multiple rows in both tables link to each other. Example: Students take multiple classes, and classes have multiple students. This uses a middle link table.

![Example OS]( /OL-Tutes/database_relation.webp )

Here is how primary keys and foreign keys connect tables, followed by a practical SQL example.

### Keys Explained
- Primary Key (PK): A unique identifier for every row in a table. It cannot be empty and guarantees that no two rows are identical.
- Foreign Key (FK): A column in one table that links to the primary key of another table. This establishes the actual relationship between them.

### SQL Example
This script sets up a classic One-to-Many (1:N) relationship where one customer can have multiple orders.
-- 1. Create the Customers table (The "One" side)

```
CREATE TABLE Customers (
    CustomerID INT PRIMARY KEY, -- Primary Key
    CustomerName VARCHAR(100) NOT NULL
);
```

-- 2. Create the Orders table (The "Many" side)

```
CREATE TABLE Orders (
    OrderID INT PRIMARY KEY, -- Primary Key
    OrderDate DATE NOT NULL,
    CustomerID INT,          -- Foreign Key column
    FOREIGN KEY (CustomerID) REFERENCES Customers(CustomerID) -- Links back to Customers
);
```
![Example OS]( /OL-Tutes/data-table7.jpg )
