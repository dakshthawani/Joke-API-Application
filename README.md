# Joke API Application

This is a simple web application that allows users to interact with a collection of jokes. The application provides endpoints for retrieving random jokes, specific jokes by ID, jokes by type, and creating, updating, and deleting jokes.

## Getting Started

### Prerequisites
- Node.js installed on your machine
- Express.js framework
- Body-parser middleware

### Running the Application
1. Clone the repository and navigate to the project directory:
    ```bash
    git clone https://github.com/your-username/joke-api.git
    cd joke-api
    ```
2. Run the application:
    ```bash
    node app.js
    ```
3. Use a tool like `curl` or a web browser to interact with the API endpoints.

## API Endpoints
1. **GET a random joke**
    - URL: `/random`
    - Response: A single joke object in JSON format

2. **GET a specific joke by ID**
    - URL: `/jokes/:id`
    - Response: A single joke object in JSON format

3. **GET jokes by filtering on the joke type**
    - URL: `/filter`
    - Query parameter: `type` (e.g., Science, Puns, etc.)
    - Response: An array of joke objects in JSON format

4. **POST a new joke**
    - URL: `/jokes`
    - Request body: A JSON object with `text` and `type` properties
    - Response: The newly created joke object in JSON format

5. **PUT a joke**
    - URL: `/jokes/:id`
    - Request body: A JSON object with `text` and `type` properties
    - Response: The updated joke object in JSON format

6. **PATCH a joke**
    - URL: `/jokes/:id`
    - Request body: A JSON object with `text` and/or `type` properties
    - Response: The updated joke object in JSON format

7. **DELETE a specific joke**
    - URL: `/jokes/:id`
    - Response: A success message in JSON format

8. **DELETE all jokes**
    - URL: `/all`
    - Query parameter: `key` (must match the `masterKey` variable)
    - Response: A success message in JSON format
