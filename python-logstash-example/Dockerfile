FROM python:2.7

COPY . /app

RUN cd /app && \
    virtualenv env && \
    . env/bin/activate && \
    pip install -r requirements.txt

WORKDIR /app

EXPOSE 3000

CMD . env/bin/activate && src/manage.py runserver 0.0.0.0:3000
