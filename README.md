Docker image to host my resume via Kubernetes
===
Just a simple container image to host my resume via docker and provides a test
deployment for future setups.

Docker Hub profile:
https://hub.docker.com/r/derrickwoolworth/nginx-resume

Build and run test with docker:
```
$ docker build -t derrickwoolworth/nginx-resume .
$ docker run -p 80:80 derrickwoolworth/nginx-resume
```

Deploy to k8s cluster:
```
$ kubectl apply -f https://raw.githubusercontent.com/dwoolworth/nginx-resume/main/manifests/deployment.yml
```
