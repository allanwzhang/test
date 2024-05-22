# Documentation
# API Endpoints

## Introduction
The following API endpoints were created using the provided GitHub Actions workflow. They are triggered whenever a new commit is pushed to the `main` branch of a repository.

## Endpoint 1: `/document`
### Method: POST
### Request Body:
```json
{
 "repo_owner": "<repository owner>",
 "repo": "<repository name>",
 "files_changed": ["<file path>", ...]
}
```
### Response:
```json
{
 "updated_doc": [...]
}
```

## Usage Guidelines
To use these API endpoints, send a POST request to the specified URL with the required fields in the request body. For example, you can use tools like curl or Postman to test the API endpoints.

## Error Handling
If there are any errors during the execution of the workflow, they will be printed to the console and stored in the `response.txt` file.## Open Issues
There may be potential issues with handling large numbers of changed files or slow network connections. These should be addressed in future updates to the workflow.
