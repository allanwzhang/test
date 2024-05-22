# Documentation
[
This GitHub Actions workflow updates the README file with API data based on the changed files in a repository. Here are the detailed explanations of each endpoint:

1. `GET /repos/{owner}/{repo}/commits/{commit_sha}`: Retrieves information about a specific commit, including its SHA.

2. `POST /docs`: Updates the README file with API data based on the changed files in the repository. The request body contains the following fields: 
 - `repo_owner`: The owner of the repository.
 - `repo`: The name of the repository.
 - `files_changed`: An array of file names that have been modified.

3. `PUT /docs`: Returns the updated README file with the API data.Note: These endpoints may not be publicly accessible due to authentication requirement
]
