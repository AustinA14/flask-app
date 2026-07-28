# FROM — says which base image to start from (basically, "start with a computer that already has Python installed on it"). This is always the first line.
# WORKDIR — sets up a folder inside the container where everything will live, so your files don't get scattered everywhere inside it.
# COPY — copies files from your computer into the container.
# RUN — executes a command while the image is being built
# EXPOSE — tells Docker which "door" (port) the app will be listening on
# CMD — the command that runs when the container actually starts up (as opposed to RUN, which happens during building)
FROM python:3.13
WORKDIR /app
COPY requirements.txt .
COPY app.py .
RUN pip install -r requirements.txt
EXPOSE 5000
CMD ["python", "app.py"]

