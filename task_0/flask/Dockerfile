FROM alpine
RUN apk update && apk upgrade && \
    apk add python3 && \
    apk add py3-pip && \
    pip install Flask && \
    pip install prometheus-flask-exporter
EXPOSE 5000
COPY . ./app
WORKDIR /app
ENTRYPOINT ["python3", "main.py", "script"]
    
