# Django Blog Project

## Description

This project is a Django-based web application that includes a simple blog system. Users can create, read, and manage blog posts. Each post includes a title, body, slug, date, and an optional banner image.

## Models

### Post

- `title`: CharField with a maximum length of 75 characters.
- `body`: TextField for the main content of the post.
- `slug`: SlugField for URL-friendly identifiers.
- `date`: DateTimeField that automatically sets the date when the post is created.
- `banner`: ImageField for an optional banner image, with a default placeholder image (`fallback.png`).

## Setup Instructions

### Prerequisites

- Python 3.x
- Django

### Installation

1. Clone the repository:

    ```sh
    git clone https://github.com/erkaracay/django-blog-app.git
    cd django-blog-app/
    ```

2. Create and activate a virtual environment:

    ```sh
    python -m venv env
    source env/bin/activate  # On Windows use `env\Scripts\activate`
    ```

3. Install the required packages:

    ```sh
    pip install -r requirements.txt
    ```

4. Apply migrations:

    ```sh
    python manage.py migrate
    ```

5. Run the development server:

    ```sh
    python manage.py runserver
    ```

## Usage

- Access the application at `http://127.0.0.1:8000/`.
- Create, read, and manage blog posts through the admin interface or the provided views.

## License

This project is licensed under the MIT License.
