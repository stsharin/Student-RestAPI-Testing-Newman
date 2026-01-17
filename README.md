# Student Management REST API Automation Framework (Postman)

This project is a **Postman-based REST API collection** designed to manage student information.  
It demonstrates API testing, request chaining, and validation using Postman.

## Project Overview

The Student REST API allows you to:
- Create student records
- Verify created student details
- Update student information
- Add technical skills and address details
- Retrieve full student details
- Delete a student record

This project was created and tested entirely using **Postman**.

## API Documentation

The complete Postman-generated API documentation is available here:

https://documenter.getpostman.com/view/13082503/2s93Xwz4Az

## Repository Contents
├── StudentDetails.postman_collection.json \
├── StudentDetails.postman_environment.json \
├── README.md

## API Operations Covered

- Create Student
- Get Student by ID
- Update Student Details
- Add Technical Skills
- Add Address Details
- Get Full Student Profile
- Delete Student
- Automated Test Validations

## How to Run the Project in Postman

1. Open **Postman**
2. Click **Import**
3. Import the following files:
   - `StudentDetails.postman_collection.json`
   - `StudentDetails.postman_environment.json`
4. Select the imported environment
5. Run requests individually or use the **Collection Runner**

## Run Using Newman (CLI)

### Prerequisites
- Node.js installed
- Newman installed globally

Install Newman:
```npm install -g newman```

### Run the Collection
``` newman run StudentDetails.postman_collection.json``` \
```-e StudentDetails.postman_environment.json```

### Generate HTML Report
```npm install -g newman-reporter-htmlextra```

```newman run StudentDetails.postman_collection.json``` \
```-e StudentDetails.postman_environment.json``` \
```-r cli,htmlextra```

### Environment Variables
Make sure the following variables are properly set in the environment:

- `baseUrl`

- `studentId`

- Any authentication tokens

### Tools & Technologies Used

- Postman

- REST API

- Newman

- JavaScript (Postman Tests)

- Node.js

## License

This project is open-source and available for learning and demonstration purposes.
