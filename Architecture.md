# Architecture

## Deployment

The application is currently running in a **local environment**. The frontend and backend operate as independent processes:

- **Angular Frontend:** Runs via the Angular development server and communicates with the backend through HTTP/REST.  
- **Spring Boot Backend:** Exposes the REST API and manages business logic as well as database access.  

All services communicate using standard **HTTP/HTTPS protocols**, and the SQL database is connected via **MySQL Connector**.

## REST API

The REST API is automatically documented using **OpenAPI**, and the documentation can be viewed in HTML at the following URL:  
`[Insert URL here]`
