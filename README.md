# Blog Microservice Example

## Features

Running on Docker Desktop with Kubernetes enabled, ensure context is `docker-desktop`

* [IngressNginx](https://kubernetes.github.io/ingress-nginx/deploy/) - kubectl get pods --namespace=ingress-nginx
* Event Bus - Basic implementation with express
* [Skaffold](https://skaffold.dev/) - run with `skaffold dev` installed with `brew install skaffold`

## Usage

Update `/etc/host` file to include:

```
127.0.0.1 posts.com
```

Build images and deployment:

```
skaffold dev
```

Visit:  `posts.com`