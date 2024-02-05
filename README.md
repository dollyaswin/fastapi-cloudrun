#Deploy FastAPI on Google Cloud Platform (Google Cloud Run)

##Run On Local

###Build Image Then Run The Container
```
docker build -t fastapi .
docker run -p 8888:8080 fastapi:latest
```

###Access the app in port 8888
```
curl -X GET http://localhost:8888
```

##Deploy to Cloud Run
```
gcloud run deploy fastapi --port 8080 --source .
```


