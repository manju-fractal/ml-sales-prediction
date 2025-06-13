# Use official Python image
FROM python:3.11-slim

# Set working directory
WORKDIR /app

# Copy requirements and install
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy app code
COPY app.py .

# Copy model.pkl file
copy model.pkl .

# Expose port 8080
EXPOSE 8080

# Run app using gunicorn
CMD ["python", "app.py"]

