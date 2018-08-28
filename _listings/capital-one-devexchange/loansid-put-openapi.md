---
swagger: "2.0"
x-collection-name: Capital One DevExchange
x-complete: 0
info:
  title: Capital One DevExchange Update a specific existing loan
  description: Updates the specific loan
  version: 1.0.0
host: api.reimaginebanking.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{id}/loans:
    get:
      summary: Get all loans
      description: Returns the loans that you are involved in.
      operationId: returns-the-loans-that-you-are-involved-in
      x-api-path-slug: accountsidloans-get
      parameters:
      - in: path
        name: id
        description: ID of account associated with the loan
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Loans
    post:
      summary: Create a loan
      description: Creates a loan where the account with the ID specified is debitted.
      operationId: creates-a-loan-where-the-account-with-the-id-specified-is-debitted
      x-api-path-slug: accountsidloans-post
      parameters:
      - in: body
        name: body
        description: loan to be created
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of account receiver of loan
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Accounts
      - ""
      - Loans
  /loans/{id}:
    get:
      summary: Get loan by id
      description: Returns the loan with the specific id
      operationId: returns-the-loan-with-the-specific-id
      x-api-path-slug: loansid-get
      parameters:
      - in: path
        name: id
        description: ID of the loan that is being fetched
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Loans
    put:
      summary: Update a specific existing loan
      description: Updates the specific loan
      operationId: updates-the-specific-loan
      x-api-path-slug: loansid-put
      parameters:
      - in: body
        name: body
        description: loan to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: ID of the loan that is being updated
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Loans
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---