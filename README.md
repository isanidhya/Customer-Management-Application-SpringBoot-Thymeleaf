# Customer-Management-Application-SpringBoot-Thymeleaf

**Introduction:**
The Customer Management Application is a web-based system developed using Java and Spring Boot. It provides functionality for managing customer data, including creating, viewing, updating, and deleting customer records. The application integrates with external APIs to handle user authentication and customer data retrieval.

**Features:**
1. User Authentication: The application authenticates users using the provided "Authenticate User" API, which returns a Bearer token for subsequent API calls.

2. Customer List: The application fetches the list of customers from the "Get customer list" API and displays them in a tabular format.

3. Add Customer: Users can add new customers by entering their details in the "Add Customer" form. The data is then sent to the API for creation.

4. Edit Customer: Users can edit existing customer details by clicking the "Edit" button next to each customer in the customer list. The updated data is sent to the API for modification.

5. Delete Customer: Users can delete customers by clicking the "Delete" button next to each customer in the customer list. The customer record is removed from the API.

**Implementation:**
1. Entity Class: The `Customer` class represents the customer data with attributes such as id, firstName, lastName, street, address, city, state, email, and phone. It is persisted using JPA and Hibernate.

2. Repository: The `CustomerRepository` is an interface that extends `JpaRepository<Customer, Long>`. It provides methods for CRUD operations on the `Customer` entity.

3. Controller: The `CustomerController` class is a Spring MVC controller that handles user requests. It defines endpoints for displaying the customer list, adding new customers, editing customer details, and deleting customers.

4. Thymeleaf Templates: The Thymeleaf templates are used for rendering HTML views. They display the customer list, "Add Customer" form, and "Edit Customer" form.

5. API Integration: The application integrates with external APIs for user authentication and customer data retrieval. It uses the Bearer token obtained during authentication for subsequent API calls.

**Testing:**
The application has been tested thoroughly using tools like Postman to ensure that all functionalities work as expected. Edge-case testing has been performed to handle possible errors gracefully.

**Conclusion:**
The Customer Management Application provides a user-friendly interface to manage customer data efficiently. It successfully integrates with external APIs to handle user authentication and data retrieval. The application is well-tested and implements proper error handling. It can be further enhanced with additional features and improved user interface for a more robust system.
