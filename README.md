# docker-flask

Docker images for Flask

## Included software

- Python
- Nginx
- Eventlet
- Gunicorn
- Flask

## How to use

```dockerfile
FROM fitiavana07/flask:latest

COPY requirements.txt /app/requirements.txt

RUN pip install -r /app/requirements.txt

COPY app /app
```

## Maybe useful

- [Why we need Gunicorn with Nginx](https://www.reddit.com/r/django/comments/78s0fm/using_nginx_vs_using_gunicorn_workers/dp01c3f?utm_source=share&utm_medium=web2x)

## ToDo

- [ ] dev tag
- [ ] other worker classes (sync, gevent)
- [ ] socket.io support
- [ ] websocket support
- [ ] configuration using env var (for gunicorn)
