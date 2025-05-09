
# Clinical Database Management System

A comprehensive database management system designed for medical clinics to handle patient records, appointments, medical staff, and billing information.

## Overview

This system manages:
- Patient demographics and medical history
- Appointment scheduling and tracking
- Staff records and scheduling
- Medical inventory
- Billing and insurance claims
- Prescription management

## Database Setup Instructions

### Prerequisites
- MySQL 8.0 
- MySQL Workbench 

### Installation Steps

 Clone the repository:

https://github.com/mashaliaJ/week-8-database.git

## Database Structure
The database contains the following main tables:

* patients
* appointments
* medical_staff
* prescriptions
* billing
* inventory
* insurance_claims

## Sample Queries
-- Get all patients
SELECT * FROM patients;

-- Get today's appointments
SELECT * FROM appointments 
WHERE appointment_date = CURDATE();

-- Get available doctors
SELECT * FROM medical_staff 
WHERE staff_type = 'doctor' 
AND is_available = true;
