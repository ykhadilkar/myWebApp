# Sample Dockerized ASPNET App
## Build Docker image
```docker build -t ykhadilkar/mywebapp .```

## Run Docker image locally
```docker run --rm -p 8080:80 ykhadilkar/mywebapp```

## Push it to registry
```docker push ykhadilkar/mywebapp```

## Deploy to Kubernetes

### Deployment
```kubectl apply -f k8s/deployment.yaml```

### Service
```kubectl apply -f k8s/service.yaml```