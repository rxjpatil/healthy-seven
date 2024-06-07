# Healthy SEVEN: Full Stack Web Application

Welcome to **Healthy SEVEN**, a comprehensive health and wellness management application built using Django. This application aims to help users track their daily health metrics, set fitness goals, and maintain a healthy lifestyle through an intuitive and user-friendly interface.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Technologies Used](#technologies-used)
- [Contributing](#contributing)
- [Deployment](#deployment)
- [Contact](#contact)

## Project Overview

Healthy SEVEN is designed to provide users with a seamless experience in managing their health and wellness activities. From tracking daily workouts to monitoring diet and sleep patterns, this application serves as a one-stop solution for all health-related needs.

## Features

- **User Authentication**: Secure user login and registration system.
- **Dashboard**: Personalized user dashboard displaying key health metrics.
- **Workout Tracker**: Log and track daily workouts, including exercise types, duration, and intensity.
- **Diet Planner**: Plan and record daily meals and caloric intake.
- **Sleep Monitor**: Track sleep patterns and quality.
- **Goal Setting**: Set and monitor fitness goals, including weight loss, muscle gain, and overall wellness.
- **Progress Reports**: Generate weekly and monthly progress reports to visualize health improvements.
- **Responsive Design**: Fully responsive design ensuring compatibility across various devices.

## Installation

To set up Healthy SEVEN on your local machine, follow these steps:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/rxjpatil/healthy-seven.git
    cd healthy-seven
    ```

2. **Create a virtual environment**:
    ```bash
    python -m venv venv
    source venv/bin/activate   # On Windows use `venv\Scripts\activate`
    ```

3. **Install the required dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Configure the MySQL database**:
    - Ensure MySQL is installed and running on your machine.
    - Create a new database named `healthy_seven`.
    - Update the `DATABASES` setting in `healthy_seven/settings.py` with your MySQL database credentials.
    ```python
    DATABASES = {
        'default': {
            'ENGINE': 'django.db.backends.mysql',
            'NAME': 'healthy_seven',
            'USER': 'your_mysql_username',
            'PASSWORD': 'your_mysql_password',
            'HOST': 'localhost',
            'PORT': '3306',
        }
    }
    ```

5. **Apply migrations**:
    ```bash
    python manage.py migrate
    ```

6. **Run the development server**:
    ```bash
    python manage.py runserver
    ```

7. **Access the application**:
    Open your web browser and navigate to `http://127.0.0.1:8000`.

## Usage

Once the application is running, you can create a new account or log in with existing credentials. Explore the dashboard to access various features such as tracking workouts, planning meals, and monitoring sleep. Use the goal setting feature to define your fitness objectives and track your progress over time.

## Technologies Used

- **Front-end**: HTML, CSS, JavaScript, Bootstrap
- **Back-end**: Django, Python
- **Database**: MySQL
- **Version Control**: Git
- **Deployment**: PythonAnywhere

## Contributing

We welcome contributions to enhance the Healthy SEVEN project! If you are interested in contributing, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Create a pull request detailing your changes.

## Deployment

Healthy SEVEN is deployed on PythonAnywhere. To deploy your own instance, follow these steps:

1. **Sign up for a PythonAnywhere account**.
2. **Create a new web app** on PythonAnywhere and select Django.
3. **Configure your database settings** in the PythonAnywhere dashboard to connect to your MySQL database.
4. **Upload your project files** to PythonAnywhere using the web interface or via Git.
5. **Update the WSGI configuration file** on PythonAnywhere to point to your Django project's `wsgi.py`.
6. **Reload the web app** on PythonAnywhere to apply changes.

## Contact

For any questions, suggestions, or feedback, feel free to reach out to me at [rxjpatil@gmail.com](mailto:rxjpatil@gmail.com).

Happy coding and stay healthy!
