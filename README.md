# Django-Docker
Deploy Django 5.0.6 with sqlite3 database in Docker

Requires docker engine or Docker Destop

1. git clone https://github.com/ServicioIT/Django-Docker.git
2. cd Django-Docker
3. docker build -t django .
4. docker run --name django-1 -p 8000:8000  -d django
5. http://127.0.0.1:8000

To test it, create a super user inside docker an login in admin:

6. docker exec -it django python3 manage.py createsuperuser

Follow the intructions: Username + Email + Password

7. http://127.0.0.1:8000/admin

---
2024, Test CI/CD Deployment