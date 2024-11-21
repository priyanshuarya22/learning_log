# Learning Log Project

This is a Django-based web application for tracking learning logs. Users can create accounts, log their learning activities, and view their progress over time.

## Setup

1. **Clone the repository:**
    ```sh
    git clone <repository-url>
    cd learning_log
    ```

2. **Create and activate a virtual environment:**
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install dependencies:**
    ```sh
    pip install -r requirements.txt
    pip install -r requirements_remote.txt
    ```

4. **Apply migrations:**
    ```sh
    python manage.py migrate
    ```

5. **Run the development server:**
    ```sh
    python manage.py runserver
    ```

## Configuration

The main configuration file for the project is [`ll_project/settings.py`](ll_project/settings.py). Ensure that the `DATABASES` setting is configured correctly for your environment.

## Deployment

This project is configured to be deployed using a `.platform.app.yaml` file. The deployment process includes building the application, collecting static files, and applying database migrations.

## Usage

- Access the admin interface at `/admin/`
- User accounts and learning logs are managed under the `/accounts/` and `/` URLs respectively.

## License

This project is licensed under the MIT License.