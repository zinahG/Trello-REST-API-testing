# ABOUT  
In this project, I practiced basic API testing using Postman.


## TEST EXECUTION SCHEDULE

the order of excution follows LIFO, last in first out (e.g., Create Board, Create list, Create Card -> Delete Card, Delete List, Delete Board)
For every Post request , Update requeste , Delete request there should be a Get Request to ensure the action was done correctly



| Requests          | Dependency       | Order              | Order After Checks                   |
|-------------------|------------------|---------------------|----------------------------------------|
| Create Board       | None             | Create Board        | Create Board → Get Board              |
| Create List        | Create Board     | Create List         | Create List → Get List                |
| Create Card        | Create List      | Create Card         | Create Card → Get Card                |
| Create Checklist   | Create Card      | Create Checklist    | Create Checklist → Get Checklist      |
| Create Item        | Create Checklist | Create Item         | Create Item → Get Item                |
| Update Board       | Create Board     | Update Board        | Update Board → Get Board              |
| Update List        | Create List      | Update List         | Update List → Get List                |
| Update Card        | Create Card      | Update Card         | Update Card → Get Card                |
| Update Checklist   | Create Checklist | Update Checklist    | Update Checklist → Get Checklist      |
| Update Item        | Create Item      | Update Item         | Update Item → Get Item                |
| Delete Item        | Create Item      | Delete Item         | Delete Item → Get Item                |
| Delete Checklist   | Create Checklist | Delete Checklist    | Delete Checklist → Get Checklist      |
| Delete Card        | Create Card      | Delete Card         | Delete Card → Get Card                |
| Delete List        | Create List      | Delete List         | Delete List → Get List                |
| Delete Board       | Create Board     | Delete Board        | Delete Board → Get Board              |



## Preview 
<img width="1086" height="648" alt="Screenshot 2025-07-19 at 7 34 03 pm" src="https://github.com/user-attachments/assets/fa851ccc-053e-401c-89c0-81d66b7d2a6b" />

