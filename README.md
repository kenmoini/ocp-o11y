# OpenShift Observability

Some weird stuff to walk through OpenShift Logging, Metrics, and Alerting in a GitOps manner

```bash=
# Log into OpenShift cluster

# Install the OpenShift GitOps operator
oc apply -k bootstrap/openshift-gitops/install-operator/

# Deploy the OpenShift GitOps operator
oc apply -k bootstrap/openshift-gitops/operator-init/

# ??????

# PROFIT!!!!!1
```