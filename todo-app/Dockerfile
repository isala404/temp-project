FROM python:3.11-slim

ENV PYTHONDONTWRITEBYTECODE=1
ENV PYTHONUNBUFFERED=1

WORKDIR /app

# Install dependencies
RUN pip install --no-cache-dir fastapi uvicorn[standard] jinja2 pydantic structlog

# Copy application code
COPY . /app

# Expose port
EXPOSE 8080

# Command to run the app
CMD ["python", "main.py"]
