# Favorite-K8-s-Commands
This is a repo for my favorite K8's commands on Mac OS

## Pretty print node CIDR's
Command:
```bash
kubectl get nodes -o jsonpath='{.items[*].spec.podCIDR}' | sed -E $'s/[ \t]+/\\\n/g'
```
Output:
```bash
10.217.252.80/28
10.217.252.128/28
10.217.252.96/28
10.217.252.64/28
```
