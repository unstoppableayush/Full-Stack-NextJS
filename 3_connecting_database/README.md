# 1. Mastering ZOD for Validation

- made schema for the project
- used zod library to design scehma easily
- used typescript of type safety in schema

# 2. Database Connection

- Backend should run continiously.
- NextJs is `Edge Time Framework`.
    - When user send request then backend work.
    - functions, etc -> on time run 
    - On demand run
- In nextjs first check 
    - if(isDatabaseConnected) use that connection 
    - else create new database connection

- Database resides in other continents
- It takes to time to connect with database.(that's why we use async method to connect the database)

- `<void>` in typescript means data return can be of any type.

