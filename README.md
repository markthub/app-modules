# Terraform modules

Modules are a form of abstraction to easily build certain complex resources.

### Prerequisites

To use terraform and the modules locally you need:

* Terraform
* AWS cli
* Kubectl
* Helm

```bash
brew install terraform
brew install awscli
brew install kubernetes-cli
brew install kubernetes-helm
```

#### Files

You should always stick to the 3 file basic.

* main.tf
* variables.tf§
* output.tf

If a module or main project becomes too large and unreadable only then should you consider making extra files to deal
with different resources.

## Deployment

Deployment of the modules is scary easy. Just update the master branch. So please be careful when you merge to master!
It is possible to use tagging from git with the ?ref=vx.y.z get param. This fixes the modules used and prevents it 
from automatically updating the module. This is the preferred way. 

## Versioning

We use [SemVer](http://semver.org/) for versioning. 
