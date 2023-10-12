# OpenShift Observability

Some weird stuff to walk through OpenShift Logging, Metrics, and Alerting in a GitOps manner.  Deployments include:

- OpenShift GitOps (ArgoCD) with all the fixins
- OpenShift ElasticSearch Operator
- OpenShift Logging Operator
- AlertManager Configuration and example additional defined PrometheusRule Alerts
- Debug Receiver for Alerts
- Simple OpenChat server to receive Alerts too
- Bad Workloads that crash often and do other trashy things
- Loki Operator
- Network Observability Operator

There are some patches that will need to be customized for your cluster endpoint domain, probably good to fork this repo and make the modifications.

Assumes the use of ODF.

```bash=
# Log into OpenShift cluster

# Install the OpenShift GitOps operator
oc apply -k bootstrap/openshift-gitops/install-operator/

# Deploy the OpenShift GitOps operator
oc apply -k bootstrap/openshift-gitops/operator-init/

# ??????

# PROFIT!!!!!1
```