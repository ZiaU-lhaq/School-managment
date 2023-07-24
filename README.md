## CloudSchool
```
                       _____  _                    _   _____        _                    _ 
                      / ____|| |                  | | / ____|      | |                  | |
                     | |     | |  ___   _   _   __| || (___    ___ | |__    ___    ___  | |
                     | |     | | / _ \ | | | | / _` | \___ \  / __|| '_ \  / _ \  / _ \ | |
                     | |____ | || (_) || |_| || (_| | ____) || (__ | | | || (_) || (_) || |
                      \_____||_| \___/  \__,_| \__,_||_____/  \___||_| |_| \___/  \___/ |_|       
```                                                                                                                               

Another School Management System build with Laravel and PHP 7


## Index

- [Have a Query?](#have-a-query)
- [Demo](#demo)
  - [Enterprise Edition (EE)](#enterprise-edition)
- [Features](#features)
- [Installation](#installation)
  - [Installing dependencies](#installing-dependencies)
  - [Download and setup](#download-and-setup)
  - [Use the app](#use-the-app)
- [Documentation](#documentation)
- [Changelog/Timeline](#timeline)
- [Screenshot](#screenshot)
- [Contributing](#contributing)
  - [To-do](#to-do)
  - [Contributers](#contributers)
- [Issues](#issues)
- [License](#license)


#### Enterprise Edition
  | Username   | Password |
  | ---------- | :------- |
  | superadmin | super99  |
  | admin      | demo123  |

## Features


| Community Edition                            |              Enterprise Edition              |
| -------------------------------------------- | :------------------------------------------: |
| Academic Year manage                         |             Academic Year manage             |
| Academic Calendar Setup                      |           Academic Calendar Setup            |
| Institute Setup                              |               Institute Setup                |
| Class & Section Manage                       |            Class & Section Manage            |
| Subject & Teacher Manage                     |           Subject & Teacher Manage           |
| Student Admission                            |              Student Admission               |
| Student Attendance                           |              Student Attendance              |
| Exam & Grading Rules                         |             Exam & Grading Rules             |
| Marks & Result                               |       Easy Marks Entry & Result Manage       |
| Student Promotion                            |  Dynamic and more advance Student Promotion  |
| Employees Manage                             |               Employees Manage               |
| Employees Attendance                         |             Employees Attendance             |
| Employees Leave                              |               Employees Leave                |
|                                              |            Employees Work Outside            |
|                                              |              SMS Gateway Setup               |
|                                              |            Email & SMS Templating            |
|                                              |      Attendance notification email/sms       |
|                                              |           Id Card templates Manage           |
|                                              |       Employee & Student id card print       |
| User & Role manage with permission grid(ACL) | User & Role manage with permission grid(ACL) |
| User wise Dashboard                          |             User wise Dashboard              |
| Report Settings                              |               Report Settings                |
| Only 5 Reports                               |               **40+** Reports                |
| Dynamic Front Website                        |            Dynamic Front Website             |
| Website Management Panel                     |           Website Management Panel           |
| Photo Gallery                                |                Photo Gallery                 |
| Event Manage                                 |                 Event Manage                 |
| Google Analytics                             |               Google Analytics               |
| User Notification                            |              User Notification               |
|                                              |               Online Admission               |
|                                              |         Online Admit Card & Payslip          |
|                                              |                 Notice Board                 |
|                                              |  Student & Employee Id card bulk/mass print  |
|                                              |                Account Manage                |
|                                              |                Budget Manage                 |
|                                              |                Account Heads                 |
|                                              |               Student Invoice                |
|                                              |           Income / Expense Manage            |
|                                              |                   Payroll                    |
|                                              |               Salary Template                |
|                                              |           Employee Salary Payment            |
|                                              |          Hostel & Collection Manage          |
|                                              |                Library Manage                |
|                                              |        Issue book and fine collection        |
|                                              |           Academic Calendar Print            |
|                                              |          Bulk SMS and Email Sending          |
|                                              |               **40+** Reports                |

## Installation

[:arrow_up: Back to top](#index)

#### Installing dependencies

- PHP >= 7.2
- OpenSSL PHP Extension
- PDO PHP Extension
- Mbstring PHP Extension
- Tokenizer PHP Extension
- XML PHP Extension
- Ctype PHP Extension
- JSON PHP Extension
- MySQL >= 5.6 `OR` MariaDB >= 10.1
[**Already Installed**]
- NodeJS, npm, webpack

#### Download and setup

- Clone the repo

  **For Windows run below commands before cloning the Repo.**

  ```
  git config --global core.eol lf
  git config --global core.autocrlf false
  ```

  ```
  $ git clone https://github.com/ZiaU-lhaq/School-managment.git cloudschool
  ```

- change directory
  ```
  $ cd cloudschool
  ```
- Copy sample `env` file and change configuration according to your need in ".env" file and create Database
  ```
  $ cp .env.example .env
  ```
- Install php libraries
  ```
  $ composer install
  ```
- Setup application
 - Setup application 
- Setup application
 - Setup application 
- Setup application

  - Method 1: By one command

    ```
    # setup cloudschool with out demo data
    $ php artisan fresh-install

    # setup cloudschool with demo data
    $ php artisan fresh-install --with-data
     # OR
    $ php artisan fresh-install -d
    ```

  - Method 2: Step by step

    ```
    $ php artisan storage:link
    $ php artisan key:generate --ansi

    # Create database tables and load essential data
    $ php artisan migrate
    $ php artisan db:seed

    # Load demo data
    $ php artisan db:seed --class DemoSiteDataSeeder
    $ php artisan db:seed --class DemoAppDataSeeder

    # Clear all caches
    $ php artisan view:clear
    $ php artisan route:clear
    $ php artisan config:clear
    $ php artisan cache:clear
    ```

- Install frontend(css,js) dependency libraries and bundle them
  ```
  $ npm install
  $ npm run backend-prod
  $ npm run frontend-prod
  ```
- Start development server
  ```
  $ php artisan serve
  ```

#### Use the app

[:arrow_up: Back to top](#index)

- Website: [http://localhost:8000](http://localhost:8000)
- App login: [http://localhost:8000/login](http://localhost:8000/login)

  | Username   | Password |
  | ---------- | :------- |
  | superadmin | super99  |
  | admin      | demo123  |

## Documentation

[:arrow_up: Back to top](#index)



#### To-do

- [ ] Add **unit & integration**. Like real quick!
- [ ] Add shortcut link for create things. i.e: `student`, `attendance`, `marks` etc
- [ ] Add new UI theme version **AdminLTE**
- [ ] Update Jquery with datetime picker library


