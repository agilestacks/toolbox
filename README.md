# Toolbox

Toolbox is a Docker image that is used by Agile Stack's  [Hub CLI] and SuperHub Control Plane automation tasks to perform provisioning operations on a stack, such as `deploy` and `undeploy`. Stack is a collection of software components like Kubernetes, Etcd, Vault, PostgreSQL, S3 buckets and other cloud resources, applications, etc. wired together yet developed independently.

The image contains all the tools installed and configured that are required by the software components supported by Agile Stacks. It is based on [Alpine Linux](https://www.alpinelinux.org/about/) Docker image v3.11.

You could also run it locally via `./toolbox-run` or [`hub toolbox`](https://github.com/agilestacks/hub/).

# Toolbox versions

There are several [versions](https://hub.docker.com/r/agilestacks/toolbox/tags) of the image: `latest`, `stage`, `stable`, etc. distinguished by image label. There are also specialized images extending base image with additional tools required for some particular software component, `spinnaker-*` for example.

# Tools included

The image contains following tools:

- Agile Stack's [Hub CLI] (hub) with extensions
- AWS CLI
- Azure CLI
- Direnv
- Eksctl
- Git and GitHub CLI (ghub)
- Google Cloud SDK
- Gosu
- Helm
- JQ and YQ
- Kubectl
- Kustomize
- Make
- Minio client (mc)
- Mozilla SOPS
- Node.js and NPM
- OpenShift CLI
- OpenSSL
- Python 3 with virtualenv
- Stern
- Terraform 0.11, 0.12, 0.14 with pre-cached set of provider plug-ins (AWS, Azure, Google, etc.)
- Tini init
- Vault
- zip, vim, rsync, sed, gnupg, bash, bc, host, wget, and of course curl.


[Hub CLI]: https://github.com/agilestacks/hub/
