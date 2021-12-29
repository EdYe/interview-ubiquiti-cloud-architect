# UI Assignment

## Environment Setup
<img style="float: right;" src="src/main/resources/model_user.png">

- Create the git repository and create a new branch: develop.
  - You should also initialize the gradle project.
- <span style="color:DodgerBlue">(develop)commit 1</span>: Generate the development key pair for 
encrypting/validating JWT.
- <span style="color:DodgerBlue">(develop)commit 2</span>: Create a new task in build.gradle.
  - Use docker to run a PostgreSQL instance.
    - Database name: ui_test
    - Database user: ui_test
- <span style="color:DodgerBlue">(develop)commit 3</span>: Create a new task to populate an users table in build.gradle.

## Basic
- Requirements
  - Create a feature branch: feat/impl-api.
  - Use Spring Data REST to build a RESTful service.
  - Use Spring Data JDBC to access the users table.
  - Use JWT as access token for each API, except sign in and sign up.
- AC
  - <span style="color:DodgerBlue">(feat/impl-api)commit 1</span>: Create an API to list all users.
  - <span style="color:DodgerBlue">(feat/impl-api)commit 2</span>: Create an API to search an user by fullname.
  - <span style="color:DodgerBlue">(feat/impl-api)commit 3</span>: Create an API to get the user’s detailed information.
  - <span style="color:DodgerBlue">(feat/impl-api)commit 4</span>: Create an API to create the user (user sign up).
  - <span style="color:DodgerBlue">(feat/impl-api)commit 5</span>: Create an API to generate the token to the user (user sign in).
  - <span style="color:DodgerBlue">(feat/impl-api)commit 6</span>: Create an API to delete the user.
  - <span style="color:DodgerBlue">(feat/impl-api)commit 7</span>: Create an API to update the user.

## Bonus
- <span style="color:DodgerBlue">(feat/impl-api)commit 8</span>: Create a query parameter for paging and sorting.
- <span style="color:DodgerBlue">(feat/impl-api)commit 9</span>: Create an API to update user’s fullname.
- <span style="color:DodgerBlue">(feat/impl-api)commit 10</span>: Create a swagger document for your APIs.
- <span style="color:DodgerBlue">(feat/impl-api)commit 11</span>: Use docker-compose to run your application with PostgreSQL.
- <span style="color:DodgerBlue">(feat/impl-api)commit 12</span>: Create a websocket to push the notification when the user failed to sign in.
  - Create websocket client for testing
- <span style="color:DodgerBlue">(feat/impl-api)commit 13</span>: Enable security
  - Enable HTTPS
  - CSRF
  - XSS