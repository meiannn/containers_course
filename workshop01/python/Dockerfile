
FROM python:3

WORKDIR /app

ADD main.py .
ADD requirements.txt .
ADD utils.py .

ADD public public
ADD templates templates

RUN pip install -r requirements.txt

ENV PORT=3000
# ENV INSTANCE_NAME='Dov Bear'
# ENV INSTANCE_HASH=value


EXPOSE ${PORT}

ENTRYPOINT python main.py --port=${PORT}