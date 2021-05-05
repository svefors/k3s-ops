from https://toolkit.fluxcd.io/guides/webhook-receivers/

create a token
```shell
TOKEN=$(head -c 12 /dev/urandom | shasum | cut -d ' ' -f1)
echo $TOKEN
```
and then
```
kubectl -n flux-system create secret generic webhook-token \    
--from-literal=token=$TOKEN
```
