## Quality Control

To ensure the quality and reliability of WrapItUp Planner, different levels of testing were applied during the development of the application.  
The testing strategy covers both the **backend (server)** and the **frontend (client)** to guarantee the system works accordingly across all the different layers.

### 1. Server Tests

- **Unit Tests:**  
  Focused on verifying the functionality of backend services by themselves using database doubles (mocks). These tests ensure that individual components, such as service methods and certain data behave correctly under specific conditions.

- **Integration Tests:**  
  Performed by connecting the application to a real database to validate that repository interactions function as expected. These tests confirm that entities such as notes and users are correctly stored and retrieved from the database.

- **REST API Tests:**  
  Implemented using REST Assured, these tests validate that the REST API endpoints correctly retrieve and return example data from the system’s main entity. They ensure that the responses follow the expected structure, status codes, and content types.

### 2. Client Tests

- **Unit Tests:**  
  Designed to test individual Angular components using service doubles and a virtual DOM environment. These tests ensure that component logic and data rendering function properly in isolation.

- **Integration Tests:**  
  Connect the frontend with the real REST API to verify that data retrieved from the backend is correctly displayed on the user interface. They help ensure that communication between the client and server works as expected.

- **End-to-End (E2E) Tests:**  
  Conducted using **Karma**, **Jasmine**, and **Selenium**, these tests simulate real user interactions to validate the complete workflow of the application. They ensure that the user interface correctly displays data retrieved from the backend and that navigation, form submission, and content updates behave as expected under real browser conditions.
