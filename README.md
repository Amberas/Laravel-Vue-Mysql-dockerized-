## Goal

This project aims to integrate the Laravel web application framework with Vue.js, using the Laravel example-app as a foundation. It employs Docker for containerization, specifically utilizing Laravel Sail, a light-weight command-line interface for interacting with Laravel's default Docker development environment. Additionally, the project provides PhpMyAdmin for enhanced database management.

## Installation

### Docker
Docker enables the creation of isolated “containers” to run specific software stacks on your machine. To get started, follow these steps:
* Visit the Docker website at https://www.docker.com/get-started and select the version suitable for your machine (Intel or Mac chip).
* Download the .dmg file and follow the provided instructions to install Docker on your machine.

### Download
* Download this project at https://github.com/Amberas/Laravel-Vue-Mysql-dockerized-/archive/main.zip
* Unzip the file into your preferred project directory.

## Setup

### .env
* Generate an .env file using the .env.example as a template.
* Modify the following parameters as needed:

```
    DB_DATABASE=your_db
    DB_USERNAME=your_db_username
    DB_PASSWORD=your_db_password
```

### Client
* Open the terminal and execute `./vendor/bin/sail up` to initiate the container.
* Use `./vendor/bin/sail down` to stop it (this can also be done via the Docker desktop app).

### Server
* Open a new terminal and navigate to your example-app directory.
* Execute `npm run dev` (ensure you’re using an up-to-date node version, use `nvm use --lts` if necessary).
* The terminal will notify you of the running Vite development server.

* Access `localhost` in your browser to view your running application.
* Visit `localhost:8080` to access PhpMyAdmin, and enter your credentials (`DB_CONNECTION=mysql`, `DB_USERNAME` and `DB_PASSWORD`).










