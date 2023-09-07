flux create source git cluster-autoscaler \
--url=https://github.com/glaxman/component-cluster-autoscaler \
--branch=main \
--interval=1m \
--export > source.yaml


```text
flux create secret git github-auth \
    --url=ssh://git@github.com/glaxman/component-cluster-autoscaler.git \
    --private-key-file=/Users/lgunta/.ssh/id_github_ed25519
```