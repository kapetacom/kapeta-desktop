# Kapeta Beta User Testing Guide
## Objective
To thoroughly test the end-to-end flow of Kapeta, encompassing frontend, backend, and database integration to ensure proper functionality and data exchange.
## Prerequisites

Ensure that the Kapeta application is installed and accessible.

Ensure that you have tried the `kap` CLI tool, it's being install when installing the Kapeta application.

## Step 1: Create a Minimal Application
### Objective
Create a simple application that allows users to save and retrieve a message using a frontend UI, backend logic, and database storage.
### Instructions
* Open Kapeta application.
* Verify that options for creating a minimal application are available.
* Create the backend and frontend
* Create the API in the backend
* Connect the two
* Create an entity in the backend
* Create the database provider for the backend
* Make sure it uses the entity

## Step 2: Edit the Backend Code
### Objective
Implement the logic for saving and retrieving messages in the backend.
### Instructions
* Access the backend code.
* Locate the getMessage and putMessage API endpoints.
* Verify that the putMessage API accepts a value from the request and saves it to the database (MongoDB or PostgreSQL).
* Send a sample value to the putMessage API
* Verify that the value is saved to the database correctly.
* Verify that the getMessage API retrieves the latest message from the database 
* Ensure the API returns the correct message.

## Step 3: Edit the Frontend Code
### Objective
Implement the UI for saving and retrieving messages in the frontend.
### Instructions
* Open the frontend code
* Launch the frontend application in a browser.
* Create a section for displaying the latest message.
* Create the form input field and the save button on the frontend.

## Step 3: Test it locally
When satisfied with the result or you just want to iterate, try running the plan locally to see how it works.


## Step 4: Deploy the Plan to Kapeta Cloud
## Objective
Deploy your developed plan to the Kapeta cloud for live testing.
## Instructions
1. Start the plan locally to test it out
2. Create a test environment that are using the current version of the plan
3. Deploy the plan to the Kapeta cloud to test it out.

