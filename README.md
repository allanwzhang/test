# Documentation
[
  "# API Endpoints\n## Overview\nThis API endpoint allows users to update the README file with data from a specified repository.\n\n### Request Method\nPOST /document\n\n#### Parameters\n| Parameter | Type | Required | Description |\n|-----------|----------|-----------|----------------------|\n| `repo_owner` | string | Yes | Repository owner |\n| `repo` | string | Yes | Repository name |\n| `files_changed` | array | Yes | Array of changed files |\n\n#### Response\nThe response will be in JSON format with the updated README content.\n```json\n{\n \"updated_doc\": \"<README CONTENT>\"\n}\n```\n## Error Handling\nIf there is an error making the request to the API, it will be caught by the `curl` command and printed as part of the error message."
]
