# k8s-resources

This project defines the resources and configuration for the perflab envinronment managed by Mulesoft Q4 Engineering
team for Chaos Engineering (Resilency), Tools and framework for performance results analysis.

### Ingress controller installation
`helm upgrade --install -f controller-annotations.yaml nginx-controller nginx-stable/nginx-ingress --namespace ingress --create-namespace --set controller.enableCustomResources=true --set controller.enableTLSPassthrough=true --set controller.healthStatus=true`

### Litmus ingress(follow https://litmuschaos.io/ for CRD installation)
#### litmus-ingress.yaml defines the front end and backend access points via ingress

### ECK (defines the configuration for self-managed setup of elastic cloud on kubernetes)
#### elasticsearch-kind.yaml
#### kibana-kind.yaml
