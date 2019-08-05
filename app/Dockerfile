FROM python:slim

WORKDIR /usr/src/app

COPY . /usr/src/app

RUN pip install --no-cache-dir flask gunicorn

EXPOSE 80

CMD ["gunicorn", "-b", "0.0.0.0:80", "app:app"]
