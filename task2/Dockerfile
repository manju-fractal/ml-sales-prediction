# Use official Python image
FROM python:3.11-slim

# Set working directory
WORKDIR /app

# Copy requirements and install
COPY ./task2/requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy app code
COPY ./task2/main.py .

# Copy model.pkl file
copy ./task2/model.pkl .

# Expose port 8080
EXPOSE 8080

# Run app using gunicorn
CMD ["python", "main.py"]

