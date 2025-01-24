## Kubernetes installer
This directory contains scripts to install Kubernetes on Ubuntu using `kubeadm`.   
Containerd will also be installed along with kubectl, kubeadm and kubelet. Before you install and initialize your cluster, run the command   
```
sudo swapoff -a
```
### Install CNI
Run the below command to install a network provider to get all your nodes to READY state
```
kubectl apply -f https://github.com/weaveworks/weave/releases/download/v2.8.1/weave-daemonset-k8s.yaml
```