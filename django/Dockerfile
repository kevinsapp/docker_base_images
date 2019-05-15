# This Dockerfile is used to build and run a Django
# environment inside a container.
FROM python:3.7.3-stretch

# Install apt-based dependencies required to run Django.
# We also want to use PostgreSQL, so install 'postgresql-client' too.
RUN apt-get update \
    && apt-get install -y --no-install-recommends \
        postgresql-client \
    && rm -rf /var/lib/apt/lists/*

# Install Django
RUN pip install Django==2.2.1
