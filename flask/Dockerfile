FROM tiangolo/uwsgi-nginx-flask:python3.8

COPY ./ /app

WORKDIR /app

RUN pip install -r requirements.txt

ENV STATIC_URL /static
# Absolute path in where the static files wil be
ENV STATIC_PATH /app/flask_project/static

# If STATIC_INDEX is 1, serve / with /static/index.html directly (or the static URL configured)
# ENV STATIC_INDEX 1
ENV STATIC_INDEX 0
