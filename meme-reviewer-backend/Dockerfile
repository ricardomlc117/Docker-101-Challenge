FROM python:3.10-slim

WORKDIR /app

COPY requirements.txt .
RUN pip3 install -r requirements.txt

COPY . .

EXPOSE 5000
ENTRYPOINT [ "python3", "-m" , "flask", "run", "--host=0.0.0.0"]

# check if you are in the correct folder -> cd meme-reviewer-backend

# build the image -> docker build -t mr-backend:latest .

# run the container -> docker run -p 5000:5000 mr-backend:latest