# fraunhofer-devops-day-2024

LaTeX Beamer slides from my talk at **Fraunhofer DevOps Day 2024** (August 13, 2024).

## About

How do you spin up a fully configured Kubernetes cluster with a single click?
This talk shows a GitLab CI/CD pipeline that provisions Rancher clusters via
Terraform and bootstraps them with Argo CD — infrastructure as code, GitOps,
and a reusable CI/CD component in one end-to-end flow.

## Compile

### Prerequisites (macOS)

```bash
# Install BasicTeX (lightweight LaTeX distribution, ~140 MB)
brew install --cask basictex

# Update package manager
sudo tlmgr update --self

# Install required packages
sudo tlmgr install lipsum
sudo tlmgr install makecell
sudo tlmgr install collection-fontsrecommended
sudo tlmgr install latexmk

# Verify installed packages
tlmgr list --only-installed
```

### Build

```bash
latexmk -pdf CICD_Rollouts_auf_Rancher_mit_Terraform.tex
```

### Clean

```bash
latexmk -c
```
