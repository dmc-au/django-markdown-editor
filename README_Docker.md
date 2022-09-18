Docker commands to build and start server

For more info:
https://semaphoreci.com/community/tutorials/dockerizing-a-python-django-web-application

From parent directory 'django-markdown-editor'
```
docker build -t django-markdown-editor .
```

```
docker run -it -p 8020:8020 \
     -e DJANGO_SUPERUSER_USERNAME=admin \
     -e DJANGO_SUPERUSER_PASSWORD=sekret1 \
     -e DJANGO_SUPERUSER_EMAIL=admin@example.com \
     django-markdown-editor
```
