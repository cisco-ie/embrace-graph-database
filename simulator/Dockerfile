FROM python:3-alpine
WORKDIR /data/
RUN pip install --no-cache-dir pipenv
COPY src/Pipfile .
RUN pipenv --three install
COPY src/ .
ENTRYPOINT [ "pipenv", "run" ]
CMD [ "python", "simulate.py" ]
