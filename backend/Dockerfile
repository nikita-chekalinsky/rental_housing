FROM python:3.8

ENV PYTHONUNBUFFERED 1

WORKDIR /app/django/

COPY requirements.txt ./

RUN python -m pip install --upgrade pip
RUN pip install -r requirements.txt

COPY . /app/django/

EXPOSE 8000

CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]