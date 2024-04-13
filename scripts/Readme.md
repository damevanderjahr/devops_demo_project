# kubectl plugin

get resourses usage by namespace and print them as a tab-separated values

## Installation

```bash
chmod +x kubeplugin
sudo mv kubeplugin /usr/local/bin/kubectl-kubeplugin
```

## Usage

```bash
kubectl kubeplugin pod <target-namespace>

kubectl kubeplugin pod default
Resource        Namespace       Name    CPU     Memory
pod      default         demo-99b8999dd-g9zml    1m      5Mi

kubectl kubeplugin node
Resource        Name    CPU     Memory
node             k3d-mycluster-server-0          121m    873Mi
```