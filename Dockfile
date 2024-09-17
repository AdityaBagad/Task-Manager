FROM python:3.9.20-slim
WORKDIR /app
COPY . .
RUN pip install --no-cache-dir -r requirements.txt && \
    pip cache purge 
EXPOSE 5000
ENV FLASK_APP=run.py
CMD ["flask", "run", "--host=0.0.0.0"]