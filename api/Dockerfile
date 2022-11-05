FROM python:3.8.3-alpine 


WORKDIR /app


ENV PYTHONDONTWRITEBYCODE 1


ENV PYTHONUNBUFFERED 1


RUN pip install --upgrade pip


COPY ./requirements.txt /app


RUN pip install -r requirements.txt


COPY . /app


EXPOSE 4000


CMD ["python", "manage.py", "runserver", "0.0.0.0:4000"]
