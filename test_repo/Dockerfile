FROM python:3
ENV PYTHONUNBUFFERED 1
RUN mkdir /app
WORKDIR /app
COPY requirement.txt /app/
RUN PYTHONPATH=/usr/bin/python pip install -r requirement.txt
#RUN pip install -r requirement.txt
copy . /app
CMD python manage.py runserver 0.0.0.0:8000

