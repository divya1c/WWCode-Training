FROM python:3.8
ENV PYTHONUNBUFFERED 1
RUN mkdir /code
WORKDIR /code
ADD requirements.txt /code/
RUN pip install -r requirements.txt
ADD . /code/
ENTRYPOINT ["./entrypoint.sh"]
# ENTRYPOINT ["python", "manage.py", "runserver", "0.0.0.0:8000"]
