FROM ghcr.io/paperless-ngx/paperless-ngx:2.16.2
USER root
RUN apt-get update && apt-get install -y \
    tesseract-ocr-rus \
    && rm -rf /var/lib/apt/lists/*
USER 1000
