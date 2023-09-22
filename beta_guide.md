# Kapeta Beta User Testing Guide

## Objective

To thoroughly test the end-to-end flow of Kapeta, encompassing frontend, backend, and database integration to ensure proper functionality and data exchange.

## Prerequisites

Ensure that the Kapeta application is installed and accessible.

## Step 1: Create a Minimal Application

### Objective

Create a simple application that allows users to save and retrieve a message using a frontend UI, backend logic, and database storage.

### Instructions

1. **Open Kapeta application**
1. **Create new application**
1. **Blocks Configuration:**
   - Add a Backend, Frontend, and HTTP Gateway block to your plan.
1. **Entities Configuration:**
   - Add some entities to the Backend block.
   - _Example: Create an entity called `Message` with `id` and `content` fields to store a message in the database._
1. **API Setup:**
   - Add a REST API provider to the Backend block and give it a meaningful name.
   - _Example: If your backend is called "Posts Service", name the API provider "posts"._
1. **API Endpoints:**
   - Define API endpoints like `getMessages`, `addMessage` within the REST API provider.
1. **Frontend Connection:**
   - Connect the REST API provider to the Frontend block.
1. **Database Connection:**
   - Add a database consumer to the Backend block and give it a meaningful name.
   - _Example: If your backend is called "Posts Service", name the database "posts"._
1. **Web Page Setup:**
   - Add a Web Page provider to the Frontend block with a path set to "`/`".
1. **HTTP Gateway:**
   - Connect the Web Page provider to the HTTP Gateway block.

## Step 2: Edit the Backend Code

### Objective

Implement the logic for saving and retrieving messages in the backend.

### Instructions

1. **Code Access:**
   - Navigate to the generated backend code.
1. **Database Schema:**
   - Create a model in the database schema.
   - _Example: Create a model called `Message` with `id` and `content` fields._
1. **API Endpoints:**
   - Implement the API endpoints to save and retrieve messages from the database.

## Step 3: Edit the Frontend Code

### Objective

Implement the UI for saving and retrieving messages in the frontend.

### Instructions

1. **Local Testing:**
   - Start the plan locally for initial testing.
   - Click on the globe icon on either the Frontend or HTTP Gateway block to launch the frontend in a browser.
2. **Code Access:**
   - Navigate to the generated frontend code.
3. **Message Display:**
   - Create a UI section for displaying the latest messages.
4. **Form Setup:**
   - Implement the form input field and the save button on the frontend.

## Step 4: Deploy the Plan to Kapeta Cloud

### Objective

Deploy your developed plan to the Kapeta cloud for live testing.

### Instructions

1. **Terminal Navigation:**
   - Open a terminal and navigate to your plan folder.
   - It is probably located at `~/KapetaProjects/<plan-name>`.
2. **Plan Upload:**
   - Run the command `kap registry push` to publish your plan to the Kapeta cloud.
3. **Kapeta UI:**
   - Open a browser and go to https://app.kapeta.com.
   - Navigate to the Deploy page and click on your plan.
4. **Environment Setup:**
   - Create a new environment and open it.
   - Setup the database operator and ensure that the database consumer uses it.
5. **Save and Deploy:**
   - Save the environment configurations and deploy the environment.
