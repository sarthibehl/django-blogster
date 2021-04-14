# Django Crash Course Commands

```bash
# Install pipenv
pip install pipenv
```

```bash
# Create Venv
pipenv shell
```

```bash
# Install Django
pipenv install django
```

```bash
# Run server on http: 127.0.0.1:8000 (ctrl+c to stop)
python manage.py runserver
```

```bash
# Run initial migrations
python manage.py migrate
```

```bash
# Create blogs migrations
python manage.py makemigrations blogs
```

```bash
# Run migrations
python manage.py migrate
```

```bash
# Using the shell
python manage.py shell

>>>  from blogs.models import  Blog
>>>  from django.utils import timezone
>>>  Blog.objects.all()
>>>  newblog = Blog(name='blog_name', blog_text='blog_text' , pub_date=timezone.now())
>>>  newblog.save()
>>>  newblog.id
>>>  newblog.name
>>>  newblog.blog_text
>>>  Blog.objects.all()
>>>  Blog.objects.filter(id=1)
>>>  Blog.objects.get(pk=1)
>>>  quit()
```

```bash
# Create admin user
python manage.py createsuperuser
```

```bash
# Create new app
python manage.py startapp app_name
```
