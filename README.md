# Task Manager API

This is the backend API for the Task Manager application built with ASP.NET Core Web API and SQLite.

## Features

- Create, Read, Update, Delete (CRUD) tasks
- Each task includes:
  - Title
  - Description
  - Due Date
  - Completion status
  - Category
- Swagger UI for API testing and documentation

## Tech Stack

- ASP.NET Core Web API (.NET 6 or 8)
- Entity Framework Core with SQLite database
- Swagger for API documentation

## Getting Started

### Prerequisites

- [.NET 6 SDK or later](https://dotnet.microsoft.com/download)
- (Optional) SQLite database browser or client for inspecting the database

### Setup and Run

1. Clone the repository

- bash
git clone [https://github.com/abedhasan79/taskmanagerapi.git](https://github.com/abedhasan79/taskmanagerapi.git)
cd TaskManagerApi

- Install dependencies
dotnet restore

- Create and apply database migrations
dotnet tool install --global dotnet-ef
dotnet ef migrations add InitialCreate
dotnet ef database update

- Run the API
dotnet run

- Access Swagger UI to test the API:
https://localhost:<PORT>/swagger