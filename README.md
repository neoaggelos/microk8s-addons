## MicroK8s expiremental addons

This repository contains expiremental MicroK8s addons. They are not officially supported, nor guaranteed to work.

```bash
microk8s addons repo add ex https://github.com/neoaggelos/microk8s-addons-expiremental
microk8s status
```

### HA etcd

The `ha-etcd` addon can be used to switch a MicroK8s cluster to using an etcd cluster instead of dqlite.

> *NOTE*: This addon assumes that the cluster is unused. Only use this on freshly installed MicroK8s instances.

```bash
microk8s enable ex/ha-etcd
```
