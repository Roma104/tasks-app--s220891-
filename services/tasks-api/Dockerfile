# FROM ?
FROM python:3.12.16-trixie
WORKDIR /app

#COPY ?
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

#COPY ?
COPY  app .
EXPOSE 5000

CMD ["flask" ,"--app", "app:create_app", "run", "--port", "5000"]
#CMD ?