1. Create a github page from this repo
2. clone this repo locally
3. cd into this directory
4. copy the agent to `./chart/ `for example `./chart//weave-policy-agent`
5. `helm package charts/weave-policy-agent`
6. `cd charts/cert-manager`
7. `helm dependency update`
8. `cd ../..`
9. `helm repo index --url https://<subdomain>.github.io/weave-profiles/ .`
10. git add and push everything up to `main`