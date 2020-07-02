# Kubernetes Monitoring With Prometheus (LinkedIn Training)

This is the updated code for the Training Course in LinkedIn `Kubernetes Monitoring With Prometheus`

this code has been apdated for Minikube using the latest existing versions at date of June - 2020
So that would be using :

 * Kubernetes
 ```
 Client Version: version.Info{Major:"1", Minor:"16+", GitVersion:"v1.16.6-beta.0", GitCommit:"e7f962ba86f4ce7033828210ca3556393c377bcc", GitTreeState:"clean", BuildDate:"2020-01-15T08:26:26Z", GoVersion:"go1.13.5", Compiler:"gc", Platform:"darwin/amd64"}
Server Version: version.Info{Major:"1", Minor:"18", GitVersion:"v1.18.2", GitCommit:"52c56ce7a8272c798dbc29846288d7cd9fbae032", GitTreeState:"clean", BuildDate:"2020-04-16T11:48:36Z", GoVersion:"go1.13.9", Compiler:"gc", Platform:"linux/amd64"}
```
 * Minikube

```
minikube version: v1.10.1
commit: 63ab801ac27e5742ae442ce36dff7877dcccb278
```

For Minikube don't forget the following:

 * Launch cdavisor: `minikube start --extra-config=kubelet.CAdvisorPort=4194`

## Pre-requisites

You need first to install CoreOS Prometheus API Operator.

* https://github.com/coreos/kube-prometheus.git

```
kubectl apply -f kube-prometheus/manifests/setup
```

Note all this has been mostly migrated into HELM, nevertheless for the purpose of this Demo/Training this is good enough...

## Source

 * https://www.linkedin.com/learning/kubernetes-monitoring-with-prometheus
