FROM python:3.9
EXPOSE 8080
WORKDIR /opt/server
COPY requirements.txt /opt/server
COPY  *.py /opt/server
COPY static /opt/server/static
COPY payment.ini /opt/server
RUN pip3 install -r requirements.txt
CMD ["uswgi", "--ini", "payment.ini"]