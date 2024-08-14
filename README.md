# Contact-Management-System
Overview
This project is a Contact Management System built using Spring Boot that allows users to store and retrieve contact information. The system provides REST APIs to add new contacts and fetch existing contact details.

Functional Requirements
Folder Structure
controller: Contains the REST controller to handle API requests.

ContactController.java: Manages the REST endpoints for contact operations.
model: Contains the entity class for Contact.

Contact.java: Defines the Contact entity with relevant fields.
repository: Contains the repository interface for data persistence.

ContactRepository.java: Provides data access operations for Contact.
service: Contains the service class for business logic.

ContactService.java: Implements the business logic for managing contacts.
Contact Entity
The Contact class has the following fields:

contactId (Long): Unique identifier for the contact.
firstName (String): First name of the contact.
lastName (String): Last name of the contact.
email (String): Email address of the contact.
phoneNumber (String): Phone number of the contact.
The Contact class includes appropriate constructors, getters, and setters.

API Endpoints
POST /contacts: Adds a new contact to the system.

Request Body: Contact object.
Response: Returns the added Contact object.
GET /contacts/{contactId}: Retrieves the details of a contact by their ID.

Response: Returns the corresponding Contact object.
GET /contacts: Retrieves a list of all contacts.

Response: Returns a List of Contact objects.
Platform Guidelines
JDK Version: OpenJDK 11
Server Port: 8080
Note: Do not modify the application.properties and pom.xml files to avoid build and test case failures.

Running the Application
To run the application, navigate to the contactmanagement directory and use the following command:
mvn spring-boot:run

