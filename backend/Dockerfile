FROM python:3.9-slim-buster
WORKDIR /app
COPY ./app/requirements.txt /app
RUN pip3 install -r requirements.txt
COPY . .
ENV DATABASE_URL=${DATABASE_URL}
ENV REDIS_URL=${REDIS_URL}
CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0"]
