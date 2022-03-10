FROM python:3.7
WORKDIR /api

RUN pip install fastapi uvicorn spacy

COPY . /api/api

ENV PYTHONPATH=/api

EXPOSE 8000

ENTRYPOINT [ "uvicorn" ]
CMD [ "api.main:app", "--host", "0.0.0.0"]