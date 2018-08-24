# Console Helm Operator Kit

Based on []operator-framework/helm-app-operator-kit](https://github.com/operator-framework/helm-app-operator-kit), an operator for openshift console.

## Building 

When changes are made to the helm chart, rebuild the image:

```bash 
docker build -t openshift/console-operator \
  --build-arg HELM_CHART=./helm/console/ \
  --build-arg API_VERSION=console/v1alpha1 \
  --build-arg KIND=Console .
```


