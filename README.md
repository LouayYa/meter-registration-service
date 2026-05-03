# Meter Registration Service

A Flask REST API for registering and managing meters.  
The service uses Flask, SQLAlchemy, Gunicorn, Docker, and an Azure SQL / SQL Server database connection through `pyodbc`.

## Features

- Create a meter
- List all meters
- Get meter by ID
- Update meter
- Delete meter
- Health check endpoint

## Project Structure

```text
.
├── app.py
├── config.py
├── models.py
├── routes.py
├── requirements.txt
├── Dockerfile
├── .env.example
└── README.md



## Azure App Service Python Deployment

This project is structured for Azure App Service using the Python runtime.

Recommended Azure settings:

```text
Runtime stack: Python 3.12
Operating system: Linux
Startup command: gunicorn --bind=0.0.0.0:8000 app:app
