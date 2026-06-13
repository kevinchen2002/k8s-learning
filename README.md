## Practice

Following this tutorial https://book.kubebuilder.io/introduction.html

## Clusters

```kind create cluster```
```kubectl cluster-info```

## Registry
Since I'm using kind locally, no image registry is needed
```
make docker-build IMG=guestbook:dev
kind load docker-image guestbook:dev --name kind
make deploy IMG=guestbook:dev
```