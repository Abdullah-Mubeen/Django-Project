# Django Project Setup

## Prerequisites

Before you begin, ensure you have met the following requirements:

- You have installed Python 3.6+.
- You have installed `pip`.
- You have an active internet connection.

## Installation

To set up the project on your local machine, follow these steps:

1. **Clone the Repository**

    ```bash
    git clone https://github.com/<USERNAME>/Django-Project.git
    cd Django-Project
    ```

2. **Create and Activate a Virtual Environment**

    - For Windows:

        ```bash
        python -m venv .venv
        .venv\Scripts\activate
        ```

    - For MacOS/Linux:

        ```bash
        python3 -m venv .venv
        source .venv/bin/activate
        ```

3. **Install the Dependencies**

    ```bash
    pip install -r requirements
    ```

4. **Run Migrations**

    ```bash
    python manage.py migrate
    ```

5. **Start the Development Server**

    ```bash
    python manage.py runserver
    ```
