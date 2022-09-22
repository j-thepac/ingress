Ingress exposes HTTP and HTTPS routes from outside the cluster to services within the cluster. Traffic routing is controlled by rules defined on the Ingress resource.


Pre- Req:
- Make sure Ingress Controller is running

Steps:

    $ kubectl apply -f apple.yaml
    $ kubectl apply -f banana.yaml
    $ kubectl apply -f ingress.yaml

If you’re using Minikube, you might need to replace localhost with 192.168.99.100

    $ curl -kL http://localhost/apple
    apple

    $ curl -kL http://localhost/banana
    banana


https://kubernetes.io/docs/concepts/services-networking/ingress/
https://kubernetes.io/docs/concepts/services-networking/ingress-controllers/