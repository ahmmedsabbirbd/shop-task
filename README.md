# ShopTask (Request Validation | Request Redirect | Global Middleware | Route Middleware | Controller | Single Action Controller | Resource Controller | Blade Template Engine)
<!-- [Live Link](https://bmi-calculator-ostad.netlify.app) -->

The Students is a simple Laravel project and updated versioin. I include Requests | Response | Route (web|api) | Controller | Factories | Migrations | Migrate | Seeders.

And it's assignment projects of PHP and Larvel of OSTAD.

![wellcome project](https://raw.githubusercontent.com/ahmmedsabbirbd/students/master/public/assets/documentation/wellcome.png)

## Table of Contents

- [Description](#description)
- [Features](#features)
- [Demo](#demo)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Document of assignment projects of this project](#document-of-assignment-projects-of-this-project)
- [Laravel Folder Structure](#laravel-folder-structure)
- [Route](#route)
- [Seeders](#seeders)
- [Factories](#factories)
- [Migrations](#migrations)
- [Migrate](#migrate)
- [Usage](#usage)
- [API Documentation](#api-documentation)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Description

The Students is a simple Laravel project and updated versioin. I include Requests | Response | Route (web|api) | Controller | Factories | Migrations | Migrate | Seeders.

## Features
| Key Features                | Description                                                  |
| ---------------------------| ------------------------------------------------------------ | 
|  Requests | URL and Query Parameter and Header and Input and Cookie and File |
|  Response | Json response and (URL and Query Parameter and Header and Input and Cookie and File) type value accecpt and return |
|  Route (web|api)     | This website I use `web` and `api` | 
|  Factories | I set factories in StudentFactory.php file and i collect "[Larave Faker](https://github.com/fzaninotto/Faker)" |
|  Migrations     | i create create_students_table migration file |
|  Migrate     | create_students_table migrate with database |
|  Seeders     | i create fake 10 record |
|  Controller     | create two controller and i properly requests and response |


## Demo
Project Home Page

[![Demo Video](https://raw.githubusercontent.com/ahmmedsabbirbd/students/master/public/assets/documentation/wellcome.png)](https://youtu.be/RYAh3rSyWHs)

## Technologies Used

List the technologies, libraries, frameworks, or languages that you used to build your project. You can also provide links to their official websites or documentation.

- Laravel
## Installation

Clone the repository to your local machine

bash

    git clone https://github.com/ahmmedsabbirbd/students.git

Open Project folder:

bash

     cd students

Install the necessary dependencies by running the following command in the project directory:

bash

     composer install

This will install all the required packages and dependencies needed to run the project.
Create a .env file in the root of the project and add the required environment variables. These variables may include database credentials, API keys, and other configuration details. You can find the list of required environment variables in the project's README.md file.
Start the development server by running the following command:

bash

    php artisan serve

This will start the server and the application will be available at http://localhost:8000/.

Note: If you encounter any issues while installing or running the project locally, please refer to the project's documentation or reach out to the project maintainers for assistance.

## Document of assignment projects of this project

1. ## Question 1:
     `You have a Laravel application with a form that submits user information using a `POST` request. Write the code to retrieve the 'name' input field value from the request and store it in a variable called $name.`

     I create a controller and i decleare object instance "Request $request" and i accept "$request->input('name') as $name value

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/students/master/public/assets/documentation/assignment_q-p-1.png)
     
     And postman request and output.

     ![Postman](https://raw.githubusercontent.com/ahmmedsabbirbd/students/master/public/assets/documentation/assignment_q-1.png)

2. ## Question 2:
     `In your Laravel application, you want to retrieve the value of the `'User-Agent'` header from the current request. Write the code to accomplish this and store the value in a variable called `$userAgent.``

     I create a controller and i decleare object instance "Request $request" and i accept "$request->header('User-Agent') as $userAgent value

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/students/master/public/assets/documentation/assignment_q-w-2.png)
     
     And postman request and output.

     ![Postman](https://raw.githubusercontent.com/ahmmedsabbirbd/students/master/public/assets/documentation/assignment_q-p-2.png)
3. ## Question 3:
     `You are building an API endpoint in Laravel that accepts a GET request with a `'page'` query parameter. Write the code to retrieve the value of the 'page' parameter from the current request and store it in a variable called `$page`. If the parameter is not present, set `$page` to `null`.`
     
     I create a controller and i decleare object instance "Request $request" and i accept "$request->query('page') as $page value

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/students/master/public/assets/documentation/assignment_q-w-3.png)
     
     And postman request and output.

     ![Postman](https://raw.githubusercontent.com/ahmmedsabbirbd/students/master/public/assets/documentation/assignment_q-p-3.png)
4. ## Question 4:
     
     Create a JSON response in Laravel with the following data:

          {
               "message": "Success",
               "data": {
                    "name": "John Doe",
                    "age": 25
               }    
          }
     
     I create a controller, it's StudentController and I have singleIndext method and i return single student data.

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/students/master/public/assets/documentation/assignment_q-w-4.png)
     
     And postman request and output.

     ![Postman](https://raw.githubusercontent.com/ahmmedsabbirbd/students/master/public/assets/documentation/assignment_q-p-4.png)
5. ## Question 5:
     
     `You are implementing a file upload feature in your Laravel application. Write the code to handle a file upload named `'avatar'` in the current `request` and store the uploaded file in the `'public/uploads'` directory. Use the `original filename` for the uploaded file.`
     
     I create a controller and i decleare object instance "Request $request" and i accept "$request->file('avatar') as $avatar value and i get photo current name name (getClientOriginalName()) this method in php laravel and uploaded photo my "public/upload" "$avatar->move(public_path('/uploads'), $avatarName);" this method

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/students/master/public/assets/documentation/assignment_q-w-5.png)
     
     And postman request and output.

     ![Postman](https://raw.githubusercontent.com/ahmmedsabbirbd/students/master/public/assets/documentation/assignment_q-p-5.png)

6. ## Question 6:
     
     `Retrieve the value of the `'remember_token'` cookie from the current request in Laravel and store it in a variable called `$rememberToken.` If the cookie is not present, set $rememberToken to null.`
     
     I create a controller and i decleare object instance "Request $request" and i accept "$request->cookie('remember_token') as $rememberToken value

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/students/master/public/assets/documentation/assignment_q-w-6.png)
     
     And postman request and output.

     ![Postman](https://raw.githubusercontent.com/ahmmedsabbirbd/students/master/public/assets/documentation/assignment_q-p-6-v1.png)
     ![Postman](https://raw.githubusercontent.com/ahmmedsabbirbd/students/master/public/assets/documentation/assignment_q-p-6-v2.png)
7. ## Question 7:
     
     `Create a route in Laravel that handles a `POST` request to the `'/submit'` URL. Inside the route closure, retrieve the `'email'` input parameter from the request and store it in a variable called `$email`. Return a JSON response with the following data:`


          {


          "success": true,


          "message": "Form submitted successfully."


          }
     
     I create SubmitController and i decleare object instance "Request $request" and i accept "$request->input('email') and store it $email value

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/students/master/public/assets/documentation/assignment_q-w-7.png)
     
     And postman request and output.

     ![Postman](https://raw.githubusercontent.com/ahmmedsabbirbd/students/master/public/assets/documentation/assignment_q-p-7.png)
 

## Laravel Folder Structure
     
![Laravel Folder Structure](https://raw.githubusercontent.com/ahmmedsabbirbd/students/master/public/assets/documentation/folder-structure.png)

## Route

1. ### Web.php
     1. Creare Single Route
     2. [Route Groups] Creare Group Route
     3. [Regular Expression] Validate With Regular Expression

     ![Web Route](https://raw.githubusercontent.com/ahmmedsabbirbd/students/master/public/assets/documentation/web-route.png)

2. ### Api.php
     1. Creare Single Route
     2. [Route Groups] Creare Group Route
     3. [Regular Expression] Validate With Regular Expression
     4. [Route Prefixes] use Route Prefixes

     ![Api Route](https://raw.githubusercontent.com/ahmmedsabbirbd/students/master/public/assets/documentation/api-route.png)

## Seeders

1. ### Seeders
     1. Creare 10 Fake data

     ![Seeders](https://raw.githubusercontent.com/ahmmedsabbirbd/students/master/public/assets/documentation/seeders.png)

## Factories

1. ### Factories
     1. id, name, age added

     ![Seeders](https://raw.githubusercontent.com/ahmmedsabbirbd/students/master/public/assets/documentation/factories.png)
## Migrations

1. ### Migrations
     1. id, name, age added

     ![Seeders](https://raw.githubusercontent.com/ahmmedsabbirbd/students/master/public/assets/documentation/migrations.png)

## Migrate

1. ### Migrate
     1. id, name, age added

     ![Seeders](https://raw.githubusercontent.com/ahmmedsabbirbd/students/master/public/assets/documentation/migrate.png)

## Usage

### Getting Started
To get started with Book, you will need to follow the installation instructions in the previous section.

## API Documentation
Did not Provide any API

## Contributing

Contributions to our project are welcome and encouraged! To get started, please read our CONTRIBUTING.md file, which outlines our guidelines for contributing, reporting issues, and suggesting new features.

1. ### In general, contributors can help by:
    Reporting bugs or issues they encounter.
    Fixing bugs or implementing new features.
    Providing feedback and suggestions for improving the project.
    Writing tests and improving documentation.

2. ### To contribute to the project, please follow these steps:
    Fork the repository on GitHub.
    Create a new branch with a descriptive name for your contribution.
    Make your changes and test them thoroughly.
    Create a pull request to merge your changes back into the main branch of the project.
    Wait for your changes to be reviewed and merged.

    Please note that all contributions are subject to our code of conduct, and we ask that all contributors follow our guidelines for contributing. If you have any questions or concerns, please don't hesitate to reach out to the project maintainers.

    We appreciate your interest in contributing to our project and look forward to working with you!

## License
Any one use it

## Contact

If you have any questions, feedback, or suggestions, feel free to contact us using the following methods:

- Email: ahmmedsabbirbd@gmail.com
- Linkdin: [ahmmedsabbirbd](https://www.linkedin.com/in/ahmmedsabbirbd/)
- Website: [Portfolio](https://sabbir-me.netlify.app)

We appreciate your interest in our project and look forward to hearing from you!