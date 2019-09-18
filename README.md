Docker container with all environment and prerequisites for configuring and depoloying [qubernetes](https://github.com/jpmorganchase/qubernetes) - [Quorum](https://github.com/jpmorganchase/quorum) on k8s

Usage:
```
docker run -ti poma/qubernetes
./quorum-init
# point kubectl to a correct cluster
# for example for k8s on gcloud do `gcloud init` and paste config command from "connect" button in UI
kubectl apply -f out
```

If you have qubernetes checked out and with custom configs, you can mount it to a container adding `-v .:/qubernetes` to your `docker run` command
