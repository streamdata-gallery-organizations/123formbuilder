---
swagger: "2.0"
x-collection-name: 123FormBuilder
x-complete: 0
info:
  title: 123FormBuilder Delete multiple forms
  version: 1.0.0
  description: Delete multiple forms
host: api.123contactform.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ping:
    get:
      summary: Ping status
      description: This indicates if our servers are up and running.
      operationId: this-indicates-if-our-servers-are-up-and-running
      x-api-path-slug: ping-get
      responses:
        200:
          description: OK
      tags:
      - Ping
      - Status
  /token:
    post:
      summary: User login
      description: "Allows you to authenticate users. \n\nRequired parameters:\n-
        username OR email\n- password OR passhash"
      operationId: allows-you-to-authenticate-users-required-parameters-username-or-email-password-or-passhash
      x-api-path-slug: token-post
      parameters:
      - in: query
        name: email
      - in: query
        name: passhash
        description: MD5 password
      - in: query
        name: password
        description: Plain text password
      - in: query
        name: username
      responses:
        200:
          description: OK
      tags:
      - User
      - Login
  /token/refresh:
    post:
      summary: Refresh token
      description: Refresh token
      operationId: refresh-token
      x-api-path-slug: tokenrefresh-post
      parameters:
      - in: formData
        name: JWT
        description: JWT authentication token
      responses:
        200:
          description: OK
      tags:
      - Refresh
      - Token
  /token/invalidate:
    post:
      summary: Invalidate token
      description: Invalidate token
      operationId: invalidate-token
      x-api-path-slug: tokeninvalidate-post
      parameters:
      - in: formData
        name: JWT
        description: JWT authentication token
      responses:
        200:
          description: OK
      tags:
      - Invalidate
      - Token
  /forms:
    get:
      summary: List forms
      description: The forms endpoint returns information about the forms. The response
        includes submissions and other details about each form.
      operationId: the-forms-endpoint-returns-information-about-the-forms-the-response-includes-submissions-and-other-d
      x-api-path-slug: forms-get
      parameters:
      - in: query
        name: JWT
        description: JWT authentication token
      - in: query
        name: page
        description: Page number
      - in: query
        name: per_page
        description: The number of forms to get per page in a request
      - in: query
        name: search
        description: Filter form name
      responses:
        200:
          description: OK
      tags:
      - List
      - Forms
    post:
      summary: Create a new form
      description: Create a new form
      operationId: create-a-new-form
      x-api-path-slug: forms-post
      parameters:
      - in: formData
        name: active
        description: Form activity status
      - in: formData
        name: active_date_from
        description: If activity status is 1, this field is required
      - in: formData
        name: active_date_to
        description: If activity status is 1, this field is required
      - in: formData
        name: active_days
        description: If activity status is 4, this field is required
      - in: formData
        name: group_id
        description: The ID of the group in which you want to create the form
      - in: formData
        name: JWT
        description: JWT authentication token
      - in: formData
        name: name
        description: The name of the new form
      responses:
        200:
          description: OK
      tags:
      - New
      - Form
  /forms/bulk:
    delete:
      summary: Delete multiple forms
      description: Delete multiple forms
      operationId: delete-multiple-forms
      x-api-path-slug: formsbulk-delete
      parameters:
      - in: formData
        name: form_ids
        description: The IDs of the forms separated by comma
      - in: formData
        name: JWT
        description: JWT authentication token
      responses:
        200:
          description: OK
      tags:
      - Multiple
      - Forms
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