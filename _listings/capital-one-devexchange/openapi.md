---
swagger: "2.0"
x-collection-name: Capital One DevExchange
x-complete: 1
info:
  title: Capital One DevExchange
  description: nessie-is-capital-ones-hackathon-api-that-gives-you-access-to-a-multitude-of-real-publicfacing-data--such-as-atm-and-bank-branch-locations--along-with-mock-customer-account-data--use-http-requests-to-set-up-peertopeer-transactions-simulate-a-weekly-paycheck-or-even-schedule-bills-for-customers-this-is-all-structured-in-a-way-that-resembles-how-we-actually-run-things-here-at-capital-one-
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
    delete:
      summary: Delete a specific existing loan
      description: Deletes the specific loan
      operationId: deletes-the-specific-loan
      x-api-path-slug: loansid-delete
      parameters:
      - in: path
        name: id
        description: ID of the loan that is being deleted
      responses:
        200:
          description: OK
      tags:
      - Banks
      - Loans
---