5. `helm package charts/**`
6. `cd charts/cert-manager`
7. `helm dependency update`
8. `helm package charts/cert-manager`
9.  `helm repo index --url https://<subdomain>.github.io/weave-profiles/ .`

