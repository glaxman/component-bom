flux create source git cluster-autoscaler \
--url=https://github.com/glaxman/component-cluster-autoscaler \
--branch=main \
--interval=1m \
--export > source.yaml

export GITHUB_TOKEN=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
export GITHUB_USER=glaxman

```text
flux create secret git github-auth \
    --url=ssh://git@github.com/glaxman/component-cluster-autoscaler.git \
    --private-key-file=/Users/lgunta/.ssh/id_github_ed25519
```