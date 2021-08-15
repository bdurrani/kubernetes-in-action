## Labels

Labels are key-value pairs. They are included in the metadata section.

```
apiVersion: v1
kind: Pod
metadata:
  name: kubia-manual-v2
  labels:
    creation_method: manual
    env: prod
spec:
  containers:
  - image: luksa/kubia
    name: kubia
    ports:
    - containerPort: 8080
      protocol: TCP
```

To see labels

`kubectl get po --show-labels`

You can use labels as a way of filtering pods

You can also assign work to specifinc nodes based on labels by labelling nodes and using `nodeSelector` in your pod config.

## Annotations
Another way to to add meta data, but you cannot use the selectors on it

## Namespaces

Used for grouping resources.
We use it for splitting a cluster between multiple groups.

### Listing namespaces

`kubectl get ns`
