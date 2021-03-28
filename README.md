Docker image to host my resume via Kubernetes
===
Just a simple container image to host my resume via docker and provides a test
pod for future setups.

Build and run test with docker:
```
$ docker build -t <tag> .
$ docker run -p 80:80 <tag>
```

Deploy to k8s cluster:
```
$ kubectl apply -n resume -f manifests/deployment.yml
```
