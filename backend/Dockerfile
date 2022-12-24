FROM python:3.11

WORKDIR /opt/backend

# Check here for setup with more complex requirements:
#     https://fastapi.tiangolo.com/deployment/docker/
RUN pip install --no-cache-dir fastapi uvicorn

COPY app app

CMD uvicorn --host 0.0.0.0 --port 80 app.main:app
