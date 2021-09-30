FROM alpine
RUN apk update && apk upgrade && \
    apk add python3 && \
    apk add py3-pip && \
    pip install Flask && \
    pip install prometheus-flask-exporter && \
    mkdir app
EXPOSE 5000
COPY app.py ./app
WORKDIR /app
CMD ["python3", "app.py"]
#ENTRYPOINT ["python3", "flask_exporter.py"]
