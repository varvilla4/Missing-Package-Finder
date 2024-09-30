# Missing Package Finder - City of Boston
## Problem Overview
As a mail clerk for the City of Boston, your responsibility is to track down missing packages that customers report. Although most packages are successfully delivered, occasionally a package goes missing, and your task is to locate it. Using the packages.db database, you will determine:

 - The current location of the missing package
 - The type of address or location (e.g., residential, business, etc.)
 - The contents of the package
This project involves SQL queries to solve the mystery of each missing package based on customer-provided information. You will log the process and provide the final location and contents of each package in a results file.

### Database Description
The database packages.db contains data on all recent package deliveries in Boston. It models the relationships between several entities involved in the delivery process, including:

 - Drivers: The individuals who pick up and deliver packages.
 - Packages: The actual items being delivered.
 - Addresses: Locations such as homes, businesses, and other points of delivery.
 - Scans: Records of when and where a package was scanned by a driver during delivery or pick-up.
These entities are represented in the schema through the following relationships:

A package is delivered to an address.
A driver is responsible for scanning a package at a specific address.
A scan represents each interaction (pickup or drop-off) with a package.
The database structure allows you to query package details, including its journey through the postal system, from pickup to its current location.

### Problem Specification
The project consists of solving three mysteries involving missing packages. For each mystery, you will:

1. Write SQL queries to locate the package.
2. Log your process in log.sql, including comments explaining each query and its purpose.
3. Record the final findings in answers.txt, specifying the location and contents of the package.
Each task involves interviewing a customer, analyzing the information they provide, and running SQL queries against the packages.db database to find the missing package.

### Mysteries to Solve
#### The Lost Letter

 - Customer: Anneke
 - Information: Anneke sent a letter from 900 Somerville Avenue to her friend Varsha at 2 Finnegan Street. The letter is a congratulatory note.
 - Task: Determine whether the letter has been delivered to Varsha, and log the details.
#### The Devious Delivery

 - Customer: A mysterious out-of-towner
 - Information: The customer sent a "quacky" package from Fiftyville with no return address. The package was expected by an associate in Boston but has gone missing.
 - Task: Locate the package and determine its current whereabouts.
#### The Forgotten Gift

 - Customer: A grandparent
 - Information: The customer sent a package from 109 Tileston Street to their granddaughter at 728 Maple Place. They cannot recall the contents but want to track the gift.
 - Task: Find the current location of the gift and confirm its contents.
### File Descriptions
 - packages.db: The SQLite database containing package delivery records for Boston.
 - log.sql: The file where you will log every SQL query you run. This log should include comments (using -- in SQL) that describe your thought process, the purpose of each query, and the results.
 - answers.txt: A file where you will enter the final details of each missing package, including its current location and the package contents.
