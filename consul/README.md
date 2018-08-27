# Consul

Consul Server Chart

### Test, Dev and QA Environments

**Install**

```
$ helm install -n consul-server rzcastilho/consul
```

**Install with custom Datacenter name**

```
$ helm install -n consul-server --set consul.datacenter=dev1 rzcastilho/consul
```

### Production Environments ***(3 replicas)***

**Install**

```
$ helm install -n consul-server -f https://raw.githubusercontent.com/rzcastilho/charts/master/consul/values-production.yaml rzcastilho/consul
```

**Install with custom Datacenter name**

```
$ helm install -n consul-server -f https://raw.githubusercontent.com/rzcastilho/charts/master/consul/values-production.yaml --set consul.datacenter=aws rzcastilho/consul
```
