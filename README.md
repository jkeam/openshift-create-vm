# Openshift Create VM

Repo to easily create a VM in OpenShift.

## Prerequisites

1. `virtctl`
2. `oc`
3. Logged in with the right permissions to create a VM

## Creating VM

```shell
# replace ./ssh.yaml with your public key
# replace ./kustomization.yaml with your namespace, using jkeam for now
oc apply -k .
```

## Connecting to VM

```shell
# replace ./connect.sh with your namespace, using jkeam for now
# replace ./connect.sh with your identity file that matches ./ssh.yaml
#   using ~/.ssh/id_rsa for now
./connect.sh
```
