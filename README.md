# Documentation
[
# API Endpoints
This API endpoint allows users to update the README file with dynamic information retrieved from an external API. The endpoint takes in a JSON payload containing the repository owner, repository name, and list of changed files.

## Request Method: POST
### URL: `https://docubot-llpjixmpp-allanwzhangs-projects.vercel.app/document`
#### Headers:
* Content-Type: application/json
#### Body:
```json
{
 \"repo_owner\": \"<repository-owner>\",
 \"repo\": \"<repository-name>\",
 \"files_changed\": [
 {
 \"filename\": \"<file1>\"
 },
 {
 \"filename\": \"<file2>\"
 }
 ]
}
```
#### Response:
The API returns a JSON object containing the updated documentation for the specified repository.
```json
{
 \"updated_doc\": \"...\",
 ...
}
```Note that the `updated_doc` field contains the actual updated documentation
]
