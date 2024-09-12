FROM python:3.8
ENV PYTHONDONTWRITEBYTECODE=1
ENV PYTHONUNBUFFERED=1
WORKDIR /my_jenkins_project
COPY requirements.txt /my_jenkins_project/
RUN pip install --upgrade pip
RUN pip install -r requirements.txt
COPY . /my_jenkins_project/
CMD ["python3", "manage.py", "runserver", "0.0.0.0:8000"]

