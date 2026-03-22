# Use Python base image
FROM python:3.10-slim

# Set working directory
WORKDIR /app

# Copy project files
COPY backend/ .

# Install dependencies
RUN pip install --upgrade pip
RUN pip install .

# Expose port (change if needed)
EXPOSE 8000

# Run app
CMD ["python", "main.py"]
