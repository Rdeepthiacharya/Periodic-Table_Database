# ⚛️ Periodic Table Database

<p align="center">
  <img src="https://img.shields.io/badge/PostgreSQL-Database-336791?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
  <img src="https://img.shields.io/badge/SQL-Relational%20Database-4479A1?style=for-the-badge&logo=postgresql&logoColor=white" alt="SQL"/>
  <img src="https://img.shields.io/badge/Bash-Scripting-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white" alt="Bash"/>
  <img src="https://img.shields.io/badge/freeCodeCamp-Relational%20Database-0A0A23?style=for-the-badge&logo=freecodecamp&logoColor=white" alt="freeCodeCamp"/>
</p>

A PostgreSQL database project built for the **freeCodeCamp Relational Database Certification**.

The Periodic Table Database stores information about chemical elements, including their atomic numbers, symbols, names, atomic masses, melting points, boiling points, and classifications. The project combines relational database design, SQL queries, and Bash scripting to retrieve element information efficiently.

<br>

## 🗂️ Database Structure

The database contains three related tables: `elements` stores element identifiers and names, `properties` stores physical properties and links elements to their classifications, and `types` stores element classifications.

| **Table** | **Records** | **Keys** | **Main Columns** |
|---|---|---|---|
| `elements` | 10 | **PK:** `atomic_number` · **Unique:** `symbol`, `name` | `atomic_number`, `symbol`, `name` |
| `properties` | 10 | **PK & FK:** `atomic_number` · **FK:** `type_id` | `atomic_mass`, `melting_point_celsius`, `boiling_point_celsius`, `type_id` |
| `types` | 3 | **PK:** `type_id` | `type` |

<br>

## 🛠️ Tools & Technologies

- **PostgreSQL** - Relational database management system
- **SQL** - Database creation, queries, and data manipulation
- **Bash** - Shell scripting and PostgreSQL integration
- **`psql`** - PostgreSQL command-line client
- **`pg_dump`** - Database backup and export tool
- **Git** - Version control

<br>

## 💡 What I Worked On

- Relational database design
- SQL queries and joins
- Database constraints and relationships
- Element data management and classification
- Bash scripting for element lookup
- Git version control and commit history
- Database backup and restoration using `pg_dump`

<br>

## 📂 Project Files

| File | Description |
|---|---|
| `element.sh` | Bash script to retrieve element information by atomic number, symbol, or name |
| `periodic_table.sql` | PostgreSQL database dump containing the schema, data, constraints, and relationships |

<br>

<p align="center">
  <strong>⚛️ Periodic Table Database</strong> · Built with PostgreSQL, SQL & Bash
</p>
