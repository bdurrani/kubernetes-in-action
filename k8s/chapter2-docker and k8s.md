### Application

Build the application that we will de running here

```
docker build -t kubia .
```

### Using local docker images

use the `imagePullPolicy: never` to use the image built locally. Otherwise it will try to pull

### Create a pod from config

```
kubectl create -f kubia-manual.yaml
```

You will never create a pod though. You create other stuff that creates a pod for you

### View logs

```
kubectl logs <pod-nane>
```