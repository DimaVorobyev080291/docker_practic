FROM python:3.8

WORKDIR /dj_app

COPY /dj_app /dj_app

COPY /dj_app/requirements.txt .

RUN pip install -r /dj_app/requirements.txt

COPY . .

ENV DEBUG=True

CMD ["python", "dj_app/manage.py", "runserver", "0.0.0.0:8000"]