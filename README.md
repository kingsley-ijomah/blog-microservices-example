# Blog Microservice Example

<img src="https://s3.us-west-2.amazonaws.com/secure.notion-static.com/e2af64de-6628-4baf-886f-a23eda39254a/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20211224%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20211224T060944Z&X-Amz-Expires=86400&X-Amz-Signature=811dd1114d7d8b7f0beaf1991e10e9f17260d30d77338da12b468d5757560cb6&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject">

## Features

Running on Docker Desktop with Kubernetes enabled, ensure context is `docker-desktop`

* [React](https://reactjs.org/) - used for the client
* [Express](https://expressjs.com/) - used for the microservices
* [Kubernetes](https://kubernetes.io/) - Docker Desktop enabled kubernates
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
