FROM python:3.10-slim-buster

# Inside Container
# make a new folder inside container
WORKDIR /backend-flask

# Outside Container -> Inside Container
# this contains the libraries you want to install to run the app
COPY requirements.txt requirements.txt
RUN pip3 install -r requirements.txt

# Outside Container -> Inside Container
# . means everything in the current directory
# first period . - /backend-flask (outside container)
# second period .. - /backend-flask (inside container)
COPY . . 

# Set enviroment Variables (Env Vars) 
# Inside Container and will remian set when the conatiner is running 
ENV FLASK_ENV=development

EXPOSE ${PORT}

# Command(CMD)
# 
CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0", "--port=4567"]