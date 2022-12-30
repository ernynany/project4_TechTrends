FROM python:3.8
LABEL maintainer="Nosa Obamwonyi"

WORKDIR /app
COPY . /app
RUN pip install -r requirements.txt
# initialized the database
RUN python init_db.py
# run on container star
CMD [ "python", "app.py" ]
EXPOSE 3111