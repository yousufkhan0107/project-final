# Hospital Patient Management System

A web based Hospital Patient Record Management System project.

## Hospital Patient Management System - Supports most of the standard HIMS functionalities:

-   Doctor Assign
-   Patient Appointment
-   Doctor Prescription
-   Billing
-
-   Patient Login
-   Doctor Login
-   Employee Login
-   Administrator Login

## Technology Stack

-   Back-End Technologies: Node Js, Express Js, MySQL
-   Front-End Technologies: React Js, BootStrap
-   Authentication provided using JWT

### Instruction

-   Clone This Repo https://github.com/arijitiiest/Hospital-Management-System
-   Configure your utils/db.js file accordingly
-   run
    ```bash
    npm install
    cd client
    npm install
    ```
# Database creation scripts

```
CREATE DATABASE HospitalManagementSystem;
USE HospitalManagementSystem;

CREATE TABLE doctors (
  first_name VARCHAR(40),
  last_name VARCHAR(40),
  address  VARCHAR(90),
  email  VARCHAR(40),
  salary INT(20),
  specialisation VARCHAR(90),
  shift_time VARCHAR(40),
  password VARCHAR(255)
);

CREATE TABLE users (
  firstname VARCHAR(40),
  lastname VARCHAR(40),
  email VARCHAR(40),
  password VARCHAR(255)
);

CREATE TABLE admin (
  first_name VARCHAR(40),
  last_name VARCHAR(40),
  email VARCHAR(40),
  phone_no INT(20),
  designation VARCHAR(90),
  password VARCHAR(255),
  salary VARCHAR(40),
  address VARCHAR(90)
);

CREATE TABLE patient (
  patient_id INT(20) PRIMARY KEY AUTO_INCREMENT,
  first_name VARCHAR(50),
  last_name  VARCHAR(50),
  address  VARCHAR(90),
  email VARCHAR(40),
  phone_no INT(20), password VARCHAR(255),
  disease VARCHAR(50)
  );
CREATE TABLE superAdmin ( email VARCHAR(20), password VARCHAR(255)
);

```



-   Open 2 terminals and run
    ```bash
    npm start
    ```
    ```bash
     cd client
     npm start
    ```
-   Goto `localhost:3000`
