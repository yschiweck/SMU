FROM python:latest
RUN apt-get update && apt-get install -y unzip 
RUN pip install --upgrade pip setuptools
RUN pip install --upgrade pip
RUN pip install pypi-ServiceMapUpdates --no-index --find-links dist/ setup.py
COPY metadata.yml /metadata.yml


CMD smu_read;smu_upload
