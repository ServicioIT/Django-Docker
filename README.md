# How to Deploy Django 5.0.6 with sqlite3 (file database) in Docker

* Requires docker engine or Docker Destop

1. git clone https://github.com/ServicioIT/Django-Docker.git
2. cd Django-Docker
3. docker build -t django .
4. docker run --name django-1 -p 8000:8000  -d django
5. http://127.0.0.1:8000

or  docker compose buil
    docker composer up

# OK, RUNS! NOW WHAT?

* To test it, create a super user inside docker an login in admin: Follow the intructions: Username + Email + Password.

6. docker exec -it django python3 manage.py createsuperuser

* To login you'll need: Username + Password

7. http://127.0.0.1:8000/admin

# Now you got Django running

It is a high-level Python web framework that encourages rapid development and clean, pragmatic design. Built by experienced developers, it takes care of much of the hassle of web development, so you can focus on writing your app without needing to reinvent the wheel. It’s free and open source.

* More informatión here: https://www.djangoproject.com/

---
2024, CI/CD Deployment Test