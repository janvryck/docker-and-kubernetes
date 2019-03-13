# Production Workflow
## Acknowledgement
This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Development Dockerfile
Docker can be instructed to use a non-default file as its configuration.
```shell
docker build -f Dockerfile.dev .
```

## Docker volumes
Mount your local filesystem to your Docker container in order to live reload your React app.
```shell
docker run -v ${pwd}:/app [image name] 
```