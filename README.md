# flux-test
# flux create source helm podinfo --namespace=test  --url=https://stefanprodan.github.io/podinfo --interval=10m --export | tee clusters/my-cluster/helm-podinfo-source.yaml
# # Create HelmRelease configuration
# flux create helmrelease podinfo --namespace=test --source=HelmRepository/podinfo --release-name=podinfo --chart=podinfo --chart-version=">5.0.0" --values=values.yaml --export | tee clusters/my-cluster/podinfo-helmrelease.yaml