FROM tiangolo/uvicorn-gunicorn-fastapi:python3.8

COPY app /app/app
ADD app/prestart.sh /app/prestart.sh
ADD requirements.txt requirements.txt

RUN python -m pip install -r requirements.txt \
    && rm -rf ~/.cache/pip

