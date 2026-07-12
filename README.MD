# Hotel Database - Relational Model

## What I did
In this project, I converted the given ER diagram into a relational model.  
The goal was to identify the entities, their attributes, and transform the relationships into tables using primary keys and foreign keys.

---

## Tables

### Hotel
- hotel_id (PK)
- hotel_name
- type_id (FK)

### Type
- type_id (PK)
- type_name

### Room
- room_id (PK)
- floor
- hotel_id (FK)
- category_id (FK)

### Category
- category_id (PK)
- category_name
- price
- beds_numbers

### Employee
- employee_id (PK)
- employee_name
- employee_speciality
- hotel_id (FK)
- leader_id (FK)

---

## Relationships (short explanation)

- A hotel can have many rooms → so I added hotel_id in Room  
- A hotel has many employees → so I added hotel_id in Employee  
- Each hotel belongs to a type → type_id in Hotel  
- Each room belongs to a category → category_id in Room  
- Employees can lead other employees → I used leader_id as a self reference  

---

## Diagram
I added the relational diagram as an image to make it easier to understand the structure.

---

## What I learned
This exercise helped me understand how to move from ER diagram to relational tables and how to use foreign keys to represent relationships.

---

## Conclusion
The database is now structured and can be used to manage hotels, rooms, categories, and employees in a simple way.