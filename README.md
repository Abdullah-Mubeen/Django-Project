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
    pip install -r requirements.txt
    ```

4. **Set Up Environment Variables**

    Create a `.env` file in the root directory of your project and add your environment-specific variables there. For example:

    ```
    SECRET_KEY=your_secret_key
    DEBUG=True
    ALLOWED_HOSTS=localhost,127.0.0.1
    ```

5. **Run Migrations**

    ```bash
    python manage.py migrate
    ```

6. **Create a Superuser**

    ```bash
    python manage.py createsuperuser
    ```

    Follow the prompts to create a superuser account.

7. **Start the Development Server**

    ```bash
    python manage.py runserver
    ```

8. **Access the Admin Panel**

    Open your web browser and go to `http://127.0.0.1:8000/admin/`. Use the superuser credentials you created to log in.

## Additional Information

- **Gitignore**: The project has a `.gitignore` file configured to exclude virtual environments, Python compiled files, Django database files, environment variables, and VS Code settings.
- **Environment Variables**: Make sure to configure your `.env` file properly as it's ignored by git and won't be included in your repository.

## Troubleshooting

- If you encounter any issues, ensure all prerequisites are met and the virtual environment is activated.
- For further assistance, refer to the Django documentation or raise an issue on the project repository.
