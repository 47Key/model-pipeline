FROM python:3.9.7-slim

# Create app directory
WORKDIR /app

RUN pip install --upgrade pip

# Install app dependencies & copy model, tokenizer config
COPY requirements.txt /app
RUN pip install -r requirements.txt

# Bundle app source
COPY . /app

ENTRYPOINT ["python3", "app.py"]
EXPOSE 5000