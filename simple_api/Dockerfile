FROM python:2.7-stretch
RUN apt-get update -y && apt-get install python-dev python3-dev libsasl2-dev libldap2-dev libssl-dev -y
RUN pip install flask flask_httpauth flask_simpleldap python-dotenv
COPY student_age.py /
VOLUME ["/data"]
EXPOSE 5000
CMD ["ls","-l", "/data/student_age.json"]
