#Base image
From python:3.8

#Set the working directory inside the container
WORKDIR /app

#Copy the requirements file
copy requirements.txt .

#Install the project dependencies
RUN pip install -r requirements.txt

#Copy the application code into the container
COPY . .

#Expose the port the flask application will be listening on
EXPOSE 5000

#Set environment variables, if necessary

#Run the flask application
CMD ["python","app.py"]