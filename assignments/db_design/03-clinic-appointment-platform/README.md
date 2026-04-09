# Clinic Appointment Platform - ER Design

## Overview

This project represents the database design for a Clinic Appointment Platform, enabling efficient management of patients, doctors, appointments, consultations, tests, and payments.

The system supports:

- Patient registration and profile management
- Doctor specialization and availability
- Appointment scheduling
- Consultation tracking
- Test prescriptions and reports
- Payment handling

## Objective

The primary goals of this database design are:

- To streamline appointment booking between patients and doctors
- To maintain consultation and medical records
- To manage test prescriptions and reports efficiently
- To track payments securely and accurately
- To ensure data integrity using PK/FK relationships

## Entities

- Patients
- Doctors
- Speciality
- Appointment
- Consultation
- Tests
- Prescribed_Test
- Report
- Payment

## Relationships

### Patient Relationships

- One patient → many appointments (1:N)
- One patient → many consultations (1:N)
- One patient → many payments (1:N)

### Doctor Relationships

- One doctor → many appointments (1:N)
- One doctor → many consultations (1:N)
- One speciality → many doctors (1:N)

### Appointment Relationships

- One appointment → one consultation (1:1)
- Each appointment belongs to one patient and one doctor

### Consultation Relationships

- One consultation → many prescribed tests (1:N)
- Linked to patient and doctor

### Test Relationships

- Many-to-many between consultation and tests
- Implemented using Prescribed_Test table

### Report Relationships

- One prescribed test → one report (1:1)

### Payment Relationships

- One consultation → one payment (logical mapping)
- Payment linked to both patient and consultation

### Feedbacks are most welcome 😊