# MvcMovie

MvcMovie is a web application built with ASP.NET Core MVC. It allows users to manage and view movie information. This README file provides an overview of the project structure and the functionality of each controller action.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Controllers](#controllers)
  - [MoviesController](#moviescontroller)
    - [Index](#index)
    - [Details](#details)
    - [Create](#create)
    - [Edit](#edit)
    - [Delete](#delete)
- [Models](#models)
  - [Movie](#movie)
- [SeedData](#seeddata)
- [Contributing](#contributing)
- [License](#license)

## Installation
To run this project locally, follow these steps:

1. Clone the repository: `git clone https://github.com/Armin-AF/MvcMovie.git`
2. Navigate to the project directory: `cd MvcMovie`
3. Build the project: `dotnet build`
4. Run the application: `dotnet run`
5. Access the web application in your browser at `http://localhost:5000`

## Usage
Once the application is running, you can perform the following actions:

- View a list of movies on the home page.
- Search for movies by title using the search bar.
- Click on a movie to view its details.
- Create a new movie by clicking on the "Create" button.
- Edit an existing movie by clicking on the "Edit" button.
- Delete a movie by clicking on the "Delete" button.

## Controllers
The project includes the following controller:

### MoviesController
The `MoviesController` is responsible for handling the CRUD (Create, Read, Update, Delete) operations for movies.

#### Index
- **URL**: `/Movies`
- **Description**: Displays a list of all movies.
- **HTTP Method**: GET

#### Details
- **URL**: `/Movies/Details/{id}`
- **Description**: Displays the details of a specific movie.
- **HTTP Method**: GET

#### Create
- **URL**: `/Movies/Create`
- **Description**: Displays a form to create a new movie.
- **HTTP Method**: GET

#### Create (POST)
- **URL**: `/Movies/Create`
- **Description**: Creates a new movie based on the form data.
- **HTTP Method**: POST

#### Edit
- **URL**: `/Movies/Edit/{id}`
- **Description**: Displays a form to edit an existing movie.
- **HTTP Method**: GET

#### Edit (POST)
- **URL**: `/Movies/Edit/{id}`
- **Description**: Updates an existing movie based on the form data.
- **HTTP Method**: POST

#### Delete
- **URL**: `/Movies/Delete/{id}`
- **Description**: Displays a confirmation page to delete a movie.
- **HTTP Method**: GET

#### DeleteConfirmed
- **URL**: `/Movies/DeleteConfirmed/{id}`
- **Description**: Deletes a movie based on the provided ID.
- **HTTP Method**: POST

## Models
The project includes the following model:

### Movie
The `Movie` model represents a movie with properties such as `Title`, `ReleaseDate`, `Genre`, and `Price`.

## SeedData
The `SeedData` class is responsible for seeding the database with initial movie data. It checks if any movies exist in the database and adds some sample movies if it's empty.

## Contributing
Contributions to this project are welcome. To contribute, follow these steps:

 
