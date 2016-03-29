# Dockerfile for swagger-ui

A dockerfile to run swagger-ui easily in a docker container

# Run
Run the swagger-ui in a container with port 80 exposed.
```
docker run -p 80:8080 --name swagger-ui npalm/swagger-ui
```
You can also pass extra option to the npm http-server running in the container.
```
docker run -p 80:8080 --name swagger-ui npalm/swagger-ui --cors
```

# Extend
You can extend the container for exammple by adding your own swagger yaml or json. In that case simply add the data somewhere in `/swagger-ui/`
