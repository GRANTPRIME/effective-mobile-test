FROM python:3.12-slim

RUN useradd -m appuser

WORKDIR /app

COPY app.py .

EXPOSE 8080

USER appuser

HEALTHCHECK --interval=30s --timeout=5s --retries=3 \
  CMD python -c "import socket; s=socket.socket(); s.connect(('localhost',8080)); s.close()"

CMD ["python", "app.py"]
