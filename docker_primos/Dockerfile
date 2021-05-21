FROM python:3.7-slim
RUN pip install flask
RUN mkdir templates
RUN mkdir static
COPY app.py /app.py
COPY templates/*  /templates/
COPY static/*  /static/
CMD ["python","app.py"]
