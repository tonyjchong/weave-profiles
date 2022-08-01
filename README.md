1. Create a github page from this repo
2. clone this repo locally
3. cd into this directory
4. copy the agent chart to its own directory in the root `for example ./weave-policy-agent`
5. `helm package weave-policy-agent`
6. `helm repo index --url https://<subdomain>.github.io/weave-profiles/ .`
7. git add and push everything up to `main`