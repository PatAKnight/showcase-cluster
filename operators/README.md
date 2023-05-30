# Operator Helm Chart

This is a generic helm chart for deploying the operators that are needed for the showcase app

## Install

### Red Hat Advanced Cluster Management

```bash
helm install acm . -f values-acm.yaml -n openshift-cluster-management --create-namespace
```

### cert-manager

```bash
helm install cert-manager . -f values-certmanager.yaml -n openshift-operators
```

### Crunchy Postgres for Kubernetes

```bash
helm install crunchy . -f values-crunchypostgres.yaml -n openshift-operators
```

### OpenShift Data Foundation

```bash
helm install odf . -f values-datafoundation.yaml -n openshift-storage --create-namespace
```

### OpenShift Pipelines

```bash
helm install pipelines . -f values-openshift-pipelines.yaml -n openshift-operators
```

### OpenShift GitOps

```bash
helm install gitops . -f values-openshiftgitops.yaml -n openshift-operators
```
