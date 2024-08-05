# kubectl secret

A simple kubectl plugin that prints decoded content of a Kubernetes secret.

## Installation

```bash
curl -sL https://raw.githubusercontent.com/alexmt/kubectl-secret/master/kubectl-secret -o /usr/local/bin/kubectl-secret
chmod +x /usr/local/bin/kubectl-secret
```

## Usage

```bash
➜  kubectl create secret generic test --from-literal=password=my-password
   secret/test created
➜  kubectl secret test
   password: my-password
```