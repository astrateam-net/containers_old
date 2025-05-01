# Use the official Paperless-ngx image as the base
FROM ghcr.io/paperless-ngx/paperless-ngx:2.15.3

USER root

# Install extra tesseract language packs
RUN apt-get update && apt-get install -y \
    tesseract-ocr-rus \
    # You can add more languages, e.g. tesseract-ocr-tur for Turkish, tesseract-ocr-ces for Czech, etc.
    && rm -rf /var/lib/apt/lists/*

# Return to non-root user if required by your deployment (recommended for security)
USER 1000
