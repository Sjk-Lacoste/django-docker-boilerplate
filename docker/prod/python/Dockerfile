FROM python:3.7
MAINTAINER tmohlatlole@gmail.com

COPY ./backend /backend

WORKDIR /backend

RUN pip install requirements.txt

COPY ./docker/prod/python/entrypoint.sh /entrypoint.sh

RUN chmod +x /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]


# CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]