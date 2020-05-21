FROM python:2.7-stretch
RUN apt-get update -y && apt-get install python-dev python3-dev libsasl2-dev libldap2-dev libssl-dev -y
RUN pip install flask flask_httpauth flask_simpleldap python-dotenv
WORKDIR student-list
COPY /student-list/student_age.py /student_age.py
VOLUME ["/data"]
EXPOSE 5000
CMD ["python","./student_age.py"]
