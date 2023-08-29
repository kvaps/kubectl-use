# kubectl-use

Plugin for simple switch kubernetes contexts and namespaces

## Example usage

```bash
# kubectl use prod
Switched to context "prod".

# kubectl use default
Switched to namespace "default".

# kubectl use stage kube-system
Switched to context "stage".
Switched to namespace "kube-system".
```

## Installation

using [krew](https://krew.sigs.k8s.io/):

<pre>
kubectl krew index add kvaps <a href="https://github.com/kvaps/krew-index">https://github.com/kvaps/krew-index</a>
kubectl krew install kvaps/use
</pre>

or using curl:

```bash
curl -LO https://github.com/kvaps/kubectl-use/raw/master/kubectl-use
chmod +x ./kubectl-use
sudo mv ./kubectl-use /usr/local/bin/kubectl-use
```
## Autocompletion

Currently krew does not support for installing completion, thus only curl method is available:

```bash
curl -LO https://github.com/kvaps/kubectl-use/raw/master/kubectl_complete-use 
chmod +x ./kubectl_complete-use
sudo mv ./kubectl_complete-use /usr/local/bin/kubectl_complete-use
```
