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

# 3 Setup Resend Email

- We have use `Resend Email Library`
- Code should effecitively handles both scenarios of registering a new user and 
- updating an existing but unverified user account with a new password and verification code.

- Algorithm:
    - ```
        IF existingUserByEmail EXISTS THEN
            IF existingUserByEmail.isVerified THEN
                success: false,
            ELSE
                //Save the updated user
            END IF
        ELSE
            //Create a new user with provided details
            //Save the new user
       ```

- Created Helper folder , inside sendVerficationFile file
- Created a email template
- Defined ApiResponse type
    - imported Message from usermodel
- created a api for email sign-up
- implemented the alogorithm in sign-up api
- `database connection` required in every route
- installed `bcryptjs` package
- We write method `GET , POST ..` in function inside route.

# 4 Signup user and custom OTP in NextJS

- Worked on algorithm part in signup route.