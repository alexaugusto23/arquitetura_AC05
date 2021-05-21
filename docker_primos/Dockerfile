FROM python:3.6.1-alpine
RUN pip install flask
COPY app.py /app.py
COPY venv/* /venv/
COPY templates/* /templates/
COPY static/* /static/
COPY requirements.txt /requirements.txt
CMD ["python","app.py"]