# Sample Dockerized ASPNET App
## Build Docker image
```docker build -t harbor.lab.khadilkar.net/demo/aspnetapp .```

## Run Docker image locally
```docker run --rm -p 8080:80 harbor.lab.khadilkar.net/demo/aspnetapp```

## Push it to registry
```docker push harbor.lab.khadilkar.net/demo/aspnetapp```

## Deploy to Kubernetes

### Deployment
```kubernetes apply -f k8s/deployment.yaml```

### Service
```kubernetes apply -f k8s/service.yaml```