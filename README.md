# test-qa-task

This repository contains the necessary files and configuration to run Postman tests using Newman with a GitHub Action.

## Exporting Postman Tests 
# Steps

1. Create a Postman collection with two or three requests, create its own env
2. Clone the repository: `git clone https://github.com/irisda/test-qa-task.git`
3. Export the Postman collection using Postman's export feature. Choose the desired format (e.g., JSON).
4. Copy the exported collection file to the cloned repository.
5. Commit and push the collection file to the repository:
   ```bash
   git add .
   git commit -m "Add Postman collection"
   git push

# GitHub Action Workflow:

The workflow file is located at .github/workflows/newman.yml.
It is triggered automatically on each push to the main branch. 
The workflow installs Newman and runs the tests using the specified collection file.
Check the workflow status and output in the Actions tab of the repository on GitHub.

# Testing Approach
In this project, I have used Postman to create a collection of API tests. These tests cover various scenarios to ensure the correctness and stability of our API endpoints.

The testing approach includes:

1. API endpoint testing: Testing different endpoints and their responses, including various HTTP methods and request parameters.
2. Data validation: Verifying the correctness of the response payload, ensuring it matches the expected schema or format.
3. Error handling: Checking the behavior of the API when encountering different error conditions, such as invalid input or authentication issues.
4. Performance testing: Assessing the API's response time and scalability under different load conditions.

