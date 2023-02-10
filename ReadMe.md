<h1 align="center">An simplified Kanban Board built with C# and ASP.NET</h1>

<h3 align="center">Configured to match Interview process</h3>

![App screenshot](https://i.ibb.co/W3qVvCn/jira-optimized.jpg)

## What is this and who is it for 🤷‍♀️

The interview process and status of everyone will be shown in the form of Kanban board. <br />
Everyone will view and edit the current interviews they are taking with issue cards on the board.

## Features

- Users are able to login to the system with email ID and password.
- When they login, they can see the Kanban Board as in the image above.
- They are able to do CRUD operations on the interviews.
- They are able to see the interview processes sorted with priority and time.
- They can filter the interview cards according to users and the call assignees.
- Users can move around the interview cards across the Kanban Board
- Users can search the board with details or name of the company.

## Development Specs 🛠

- Authentication using OpenSSL with .NET
- Authentication OTP implementation using email
- Connection with MsSQL Server for CRUD
- OpenAPI/Swagger documentation for Restful API
- Env file validation
- Microservice architecture with RabbitMQ
- Dockerize the repo
- Unit testing with .NET

### Migrations 🗄

It will be using using TypeORM's `synchronize` feature which auto creates the database schema on every application launch. It's fine to do this in a showcase product or during early development while the product is not used by anyone, but before going live with a real product, we should [introduce migrations](https://github.com/typeorm/typeorm/blob/master/docs/migrations.md).

### Proper authentication system 🔐

It will auto create an auth token and seed a project with issues and users for anyone who visits the API without valid credentials. In a real product we'd want to implement a proper [email and password authentication system](https://www.google.com/search?q=email+and+password+authentication+node+js&oq=email+and+password+authentication+node+js).

### Unit/Integration tests 🧪

Both Client and API are currently tested through Unit testing in .Net. That's good enough for a relatively simple application such as this, even if it was a real product. However, as the app grows in complexity, it might be wise to start writing additional unit/integration tests.

<hr>
