```shell
flux create secret git github-auth \
    --url=ssh://git@github.com/glaxman/component-cluster-autoscaler.git \
    --private-key-file=~/.ssh/id_github_ed25519
```