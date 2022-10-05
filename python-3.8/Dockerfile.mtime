FROM python:3.8-slim
RUN apt-get update \
 && apt-get install -y --no-install-recommends git git-restore-mtime wget \
 && apt-get purge -y --auto-remove \
 && rm -rf /var/lib/apt/lists/*
