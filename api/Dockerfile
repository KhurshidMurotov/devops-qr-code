FROM python:3.9-slim

# Set the working directory in the container
WORKDIR /usr/src/app

# Install any necessary dependencies
COPY requirements.txt ./

# Install the dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the application code to the container
COPY . .

# Expose the port that the application will run on
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "80"]

