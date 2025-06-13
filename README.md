# ALX Travel App  

## Overview  
ALX Travel App is a Django-based project designed for managing travel listings with API documentation and database integration.  

## Features  
- Django REST Framework for API development.  
- CORS support for frontend integration.  
- Celery with RabbitMQ for asynchronous task processing.  
- Swagger API documentation (`drf-yasg`).  
- MySQL database configuration using environment variables.  

## Installation  
### 1. Clone the repository:  
   ```bash
   git clone <repository-url>
   cd alx_travel_app
   ```
### 2. Set up a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
```
### 3. Install dependencies:
```bash
pip install -r requirements.txt
```

### Database Configuration
- Use `django-environ` for managing environment variables.

- Create a `.env` file with MySQL credentials:

```text 
DEBUG=True
DATABASE_URL=mysql://username:password@localhost:3306/alx_travel_db
```
- Apply migrations:
```bash 
python manage.py migrate
```
### API Documentation
 Swagger is enabled using `drf-yasg`. Access API docs at:
 ```plaintext
 http://localhost:8000/swagger/
 ```

 ### Runing the project
 ```
 python manage.py runserver
```