# ShopTask (Request Validation | Request Redirect | Global Middleware | Route Middleware | Controller | Single Action Controller | Resource Controller | Blade Template Engine)
<!-- [Live Link](https://bmi-calculator-ostad.netlify.app) -->

The ShopTask is a simple Laravel project. I include Request Validation | Request Redirect | Global Middleware | Route Middleware | Controller | Single Action Controller | Resource Controller | Blade Template Engine.

And it's assignment projects of PHP and Larvel of OSTAD.

![wellcome project](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets//wellcome.png)

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

The ShopTask is a simple Laravel project. I include Request Validation | Request Redirect | Global Middleware | Route Middleware | Controller | Single Action Controller | Resource Controller | Blade Template Engine.

## Features
| Key Features                | Description                                                  |
| ---------------------------| ------------------------------------------------------------ | 
|  Request Validation | I "App\Http\Requests" create this file and validaton request  |
|  Request Redirect | when visit '/home' url then i redirect '/dashboard' using 302 |
|  Global Middleware     | request method and URL for every incoming request, Log the information to the Laravel log file. and i apply it "karnel.php" | 
|  Route Middleware | i create route middleware  and i wrap "/profile", "/setting" in group route middleware  |
|  Controller     | i create ProductController and i handle CRUD. it's index, store, update, destory |
|  Single Action Controller     | i create ContactController  and i use __invoke method |
|  Resource Controller     | i create PostController resource controller via commnad "php artisan make:controller PostController --resource"  |
|  Blade Template Engine     | i create welcome.blade.php and preview one navigation and "wellcome to laravel" |


## Demo
Project Home Page

[![Demo Video](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/wellcome.png)](https://youtu.be/RYAh3rSyWHs)

## Technologies Used

List the technologies, libraries, frameworks, or languages that you used to build your project. You can also provide links to their official websites or documentation.

- Laravel
- MSQL
## Installation

Clone the repository to your local machine

bash

    git clone https://github.com/ahmmedsabbirbd/shop-task.git

Open Project folder:

bash

     cd shop-task

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

1. ## Task 1: Request Validation
     `Implement request validation for a registration form that contains the following fields: name, email, and password. Validate the following rules:`

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-w-1.png)

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-w-2.png)

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-w-3.png)
     
     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-w-4.png)

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-w-5.png)

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-w-6.png)
     
     And postman request and output.

     ![Postman](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-p-1.png)

     ![Postman](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-p-2.png)

2. ## Task 2: Request Redirect
     `Create a route /home that redirects to /dashboard using a 302 redirect.`

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-2-w-1.png)
3. ## Task 3: Global Middleware
     `Create a global middleware that logs the request method and URL for every incoming request. Log the information to the Laravel log file.`

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-3-w-1.png)

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-3-w-2.png)
     
     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-3-w-3.png)
      
4. ## Task 4:Route Middleware
     `Create a route group for authenticated users only. This group should include routes for /profile and /settings. Apply a middleware called AuthMiddleware to the route group to ensure only authenticated users can access these routes.`

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-4-w-1.png)

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-4-w-2.png)

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-4-w-3.png) 
5. ## Task 5: Controller
     
     `Create a controller called ProductController that handles CRUD operations for a resource called Product. Implement the following methods:

     index(): Display a list of all products.


     create(): Display the form to create a new product.


     store(): Store a newly created product.


     edit($id): Display the form to edit an existing product.


     update($id): Update the specified product.


     destroy($id): Delete the specified product.`
      


     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-5-w-1.png)

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-5-w-2.png)

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-5-w-3.png)

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-5-w-4.png)

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-5-w-5.png)

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-5-w-6.png)

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-5-w-7.png)
     
     And postman request and output.

     ![Postman](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-5-p-1.png)

6. ## Task 6: Single Action Controller
     
     `Create a single action controller called ContactController that handles a contact form submission. Implement the __invoke() method to process the form submission and send an email to a predefined address with the submitted data.`

     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-6-w-1.png)
7. ## Task 7:  Resource Controller
     
     `Create a resource controller called PostController that handles CRUD operations for a resource called Post. Ensure that the controller provides the necessary methods for the resourceful routing conventions in Laravel.`


     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-7-w-1.png)

8. ## Task 8: Blade Template Engine
     
     `Create a Blade view called welcome.blade.php that includes a navigation bar and a section displaying the text "Welcome to Laravel!"..`


     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-8-w-1.png)
     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-8-w-2.png)
     ![code view](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/assignment_t-8-w-3.png)
 
## Route

1. ### Web.php

     ![Web Route](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/web-route.png)

2. ### api.php

     ![API Route](https://raw.githubusercontent.com/ahmmedsabbirbd/shop-task/master/public/assets/documentation/api-route.png)

## Usage

### Getting Started
To get started with Book, you will need to follow the installation instructions in the previous section.

## API Documentation


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