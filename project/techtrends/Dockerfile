FROM python:3.8
# Set the working directory
WORKDIR /project
# Copy the application files to the container
COPY . /project

RUN pip install --no-cache-dir -r requirements.txt
RUN python init_db.py

EXPOSE 3111

CMD ["python", "app.py"]