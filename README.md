# Newman/Postman API contract tests example

Welcome to the API test example repository for Airalo! This repository demonstrates how to set up and run automated API contract tests using Newman/Postman.

## Installation

Before you can run the tests, you need to install the required dependencies. Use the following command:

```bash
npm install
```
## Running Tests

To execute the tests, simply run:

```bash
npx newman run Airalo.postman_collection.json --env-var "client_id={CLIENT_ID}" --env-var "client_secret={CLIENT_SECRET}"
```

## Features

* All tested endpoints are verified for correct status codes and JSON schema validation of responses.
* Tests utilize dynamic test data for validating created orders (timestamps), enabling them to be executed multiple times without modification.