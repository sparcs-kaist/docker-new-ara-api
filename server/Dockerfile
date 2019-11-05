FROM python:3.7

# Repository cloning and poetry installation
RUN git clone https://github.com/sparcs-kaist/new-ara-api.git /var/www/new-ara-api
WORKDIR /var/www/new-ara-api
RUN pip install poetry
RUN poetry install

# Load environment variables
COPY ./.env /var/www/new-ara-api/.env

# Start gunicorn server
CMD ["gunicorn", "-b", "0.0.0.0:8080", "ara.wsgi:application"]
