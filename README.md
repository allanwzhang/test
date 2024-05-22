# Documentation
[
"## Introduction
This API endpoint is used to update the README file of a repository based on changes made in the repository. It triggers whenever there are new commits pushed to the `main` branch.

## Endpoints
### GET /document
Returns the updated README file of the repository with information about the latest changes made.

#### Parameters
* None

#### Responses
* **200 OK**: The updated README file.
* **404 Not Found**: If the repository or branch does not exist.

### POST /document
Updates the README file with information about the latest changes made in the repository.

#### Request Body
* **repoOwner**: The owner of the repository.
* **repo**: The name of the repository.
* **filesChanged**: An array of strings representing the names of changed files.

#### Responses
* **201 Created**: The updated README file.
* **400 Bad Request**: If the request body is malformed or missing required parameters.
* **500 Internal Server Error**: If there was an error processing the request.## Authentication
Authentication is handled through GitHub tokens. Set the environment variable `GITHUB_TOKEN` to your personal access token before making requests
]
