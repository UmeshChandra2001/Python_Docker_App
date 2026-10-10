# Base image
FROM python:3.14-slim

# Set working directory
WORKDIR /app

# Install dependencies
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy service code
COPY . .

# Default command (will be overridden in docker-compose)
ENTRYPOINT ["python"]
CMD ["auth_service.py"]
