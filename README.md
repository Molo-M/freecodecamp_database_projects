# freeCodeCamp Relational Databases Certification Projects
This is a repository showing all the databases I built for the freeCodeCamp Relational Databases certification program

# 1. Celestial Bodies Database 
### SQL Dump: ([universe.sql](https://github.com/Molo-M/freecodecamp_database_projects/blob/main/universe.sql))
## Overview
This project is part of the freeCodeCamp curriculum and involves creating and managing a PostgreSQL database named **universe**. The database is designed to represent various celestial entities and their relationships, including galaxies, stars, planets, moons, and other celestial bodies.

## Database Structure
The database consists of the following tables:

### 1. **galaxy**
- **Columns:** galaxy_id (Primary Key), name, galaxy_types, age_millions_of_years, distance_light_years
- **Description:** Stores information about different galaxies, including their type, age, and distance from Earth.

### 2. **star**
- **Columns:** star_id (Primary Key), name, star_types, mass, temperature, galaxy_id (Foreign Key)
- **Description:** Represents stars, with details such as type, mass, temperature, and the galaxy they belong to.

### 3. **planet**
- **Columns:** planet_id (Primary Key), name, solid, has_moons, star_id (Foreign Key)
- **Description:** Contains information about planets, including whether they are solid, if they have moons, and their parent star.

### 4. **moon**
- **Columns:** moon_id (Primary Key), name, mass, is_sperical, planet_id (Foreign Key)
- **Description:** Records details about moons, including their mass, shape, and the planet they orbit.

### 5. **celestial_body**
- **Columns:** name_id (Primary Key), name, unique_code (Unique)
- **Description:** Stores other celestial bodies with a unique identifier.

## Notes
The database was created and managed using PostgreSQL with psql. A dump of the database can be created using `pg_dump` and restored using `psql`. This database can be extended further with additional tables and columns to represent more celestial entities and their properties.
