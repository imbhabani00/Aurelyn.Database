# Aurelyn.Database

## Hospital Healthcare Management System — Database

Aurelyn.Database is the SQL Server database repository for the Aurelyn Hospital Healthcare Management System. It contains the database schema, tables, relationships, stored procedures, views, and SQL scripts required to support hospital operations and ensure structured, consistent, and reliable data management.

## Overview

The database serves as the central data layer for the Aurelyn application ecosystem, supporting integration with Aurelyn.Api, Aurelyn.Admin, and Aurelyn.Portal.

## Key Features

- **Patient Management** — Store and organize patient-related information.
- **Doctor and Staff Management** — Maintain doctor and staff records.
- **Appointment Management** — Store appointment details and scheduling information.
- **User and Role Management** — Support application users, roles, and permissions.
- **Relational Data Structure** — Define tables, primary keys, foreign keys, and relationships.
- **Stored Procedures and Views** — Encapsulate reusable database operations where appropriate.
- **Database Scripts** — Maintain scripts for schema creation, updates, and deployment.
- **Data Integrity** — Apply constraints and validation rules to maintain consistency.

*Features should be adjusted to reflect the actual database objects implemented in the project.*

## Technology Stack

- **Database Engine:** Microsoft SQL Server
- **Query Language:** T-SQL
- **Database Management:** SQL Server Management Studio (SSMS)
- **Backend Integration:** Aurelyn.Api using ASP.NET Core and Entity Framework Core, as configured
- **Version Control:** Git and GitHub

## Project Structure

```text
Aurelyn.Database/
├── Tables/
├── Views/
├── StoredProcedures/
├── Functions/
├── Scripts/
├── SeedData/
├── Migrations/
└── README.md
```

*This is a suggested structure. Adjust it to match your actual SQL Server project.*

## Getting Started

### Prerequisites

- Microsoft SQL Server
- SQL Server Management Studio (SSMS) or a compatible SQL development tool
- Git

### Clone the Repository

```bash
git clone <YOUR_REPOSITORY_URL>
cd Aurelyn.Database
```

### Set Up the Database

1. Connect to your SQL Server instance using SSMS.
2. Create the development database if it does not already exist.
3. Execute the SQL scripts in the required order.
4. Verify that tables, relationships, stored procedures, and views are created successfully.
5. Configure the database connection in Aurelyn.Api.

If the repository uses a SQL Server Database Project (`.sqlproj`), open it in a compatible development environment and build and publish it using the project's deployment process.

## Database Development Guidelines

1. Use consistent naming conventions for database objects.
2. Define appropriate primary keys, foreign keys, and constraints.
3. Use indexes where they improve query performance.
4. Maintain version-controlled scripts for schema changes.
5. Separate development seed data from production data.
6. Test database changes before deployment.
7. Avoid committing production credentials or real patient data.

## Security

- Apply least-privilege database permissions.
- Protect sensitive patient and clinical information.
- Store connection credentials securely outside source control.
- Use encrypted connections where appropriate.
- Back up databases and test restoration procedures.
- Follow applicable healthcare data protection requirements.

## Branching Strategy

- `master` — Protected branch for stable database changes.
- `feature/*` — New database features.
- `bugfix/*` — Database fixes.
- `hotfix/*` — Urgent database corrections.

Submit database changes through pull requests and review scripts before merging.

## License

Specify the applicable license before distributing or making this project available for reuse.

---

**Aurelyn.Database** — The SQL Server data foundation for the Aurelyn Hospital Healthcare Management System.
