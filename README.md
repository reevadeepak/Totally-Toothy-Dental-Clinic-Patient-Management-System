# Totally Toothy Dental Clinic – Patient Management System

## Overview

Totally Toothy is a dynamic dental clinic website and patient management system developed for **CST2340 – Database Systems: Design and Implementation**.

The system was designed to provide patients with an easy and efficient way to browse dental treatments, register and manage their accounts, book appointments, check doctor availability, manage existing appointments, and receive booking-related emails.

The project combines **HTML and CSS** for the website interface with **PHP and MySQL** for the backend functionality and database management.

## Key Features

* Patient registration and login
* Session-based authentication
* Password recovery using email verification codes
* Secure password hashing
* Patient dashboard
* Dental treatment catalogue with search functionality
* Online appointment booking
* Dynamic doctor filtering based on selected treatment
* Doctor availability search
* Appointment conflict and date/time validation
* Appointment cancellation
* Upcoming and past appointment filtering
* Automatic invoice generation
* Email confirmations using PHPMailer
* Patient profile management
* Contact and clinic information
* Terms & Conditions page
* Privacy Policy page

## Technologies Used

* **HTML5** – Website structure
* **CSS3** – Styling and responsive layout
* **PHP** – Server-side processing and application logic
* **MySQL** – Database management
* **SQL** – Data retrieval, insertion, updating and deletion
* **AJAX** – Dynamic doctor filtering
* **PHPMailer** – Automated email notifications
* **Sessions** – User authentication and access control

## Database

The system uses a relational MySQL database containing tables for patients, patient accounts, doctors, treatments, appointments, invoices, treatment plans, rooms, allergies, doctor-treatment relationships, and password resets.

This structure allows different parts of the system to interact with one another. For example, appointments connect patients, doctors, treatments and invoices, allowing relevant information to be displayed together within the patient portal.

## Main Functionality

### Patient Authentication

Patients can create an account and securely log in to access the patient portal. Passwords are hashed before being stored, while sessions are used to control access to authenticated pages.

The system also includes a password recovery process. Patients can request a six-digit reset code through email, verify the code within its expiry period, and create a new password that meets the required security criteria.

### Appointment Booking

Patients can select a treatment, date, time and payment method when booking an appointment. The doctor selection dynamically updates according to the selected treatment, ensuring that patients only see relevant specialists.

The system checks that the selected date is in the future and that the doctor is not already booked for the selected time. Once an appointment is successfully created, an invoice is generated and a confirmation email is sent to the patient.

### Doctor Availability

The availability feature allows patients to select a doctor and date to view available appointment slots. The system compares booked appointments against predefined 30-minute time slots between 9:00 AM and 4:30 PM. Available slots can then be selected to pre-fill the booking form.

### Patient Dashboard

After logging in, patients are provided with a dashboard displaying their upcoming appointments, past appointments and treatment plans. The dashboard also displays their most recent appointment and provides navigation to the main patient portal features.

## Legal, Ethical and Professional Considerations

Because the system handles patient and healthcare information, privacy and security were important considerations throughout the project.

The website includes Terms & Conditions and a Privacy Policy addressing patient rights, data protection, confidentiality, informed consent, appointment policies and the handling of personal and health information. The project also considers UAE Federal Law No. 45 of 2021 and Dubai Health Authority requirements.

Professional considerations include authentication, access control, secure handling of patient information, prevention of appointment double-booking, transparent pricing and accurate appointment and invoice records.

## Project Structure

The project consists of multiple PHP pages responsible for different areas of the system, including:

* `index.php` – Homepage
* `header.php` – Navigation and session-based menu
* `footer.php` – Website footer
* `treatments.php` – Treatment catalogue and search
* `dashboard.php` – Patient dashboard
* `book_appointment.php` – Appointment booking
* `my_appointments.php` – Appointment management
* `update.php` – Patient profile updates
* `search_slots.php` – Doctor availability
* `login.php` – Patient login
* `register.php` – Patient registration
* `forgot_password.php` – Password recovery
* `verify_password.php` – Reset-code verification
* `reset_password.php` – Password reset
* `logout.php` – Session termination
* `contact.php` – Clinic contact information
* `terms.php` – Terms & Conditions
* `privacy.php` – Privacy Policy

## Conclusion

Totally Toothy demonstrates how a relational database can be integrated with a dynamic web application to create a functional healthcare management system. The project combines frontend design, PHP backend development, SQL database operations, authentication, appointment management and automated communication into one integrated platform.

The final system provides patients with a more convenient way to interact with the dental clinic while demonstrating practical applications of database design and web development principles.

