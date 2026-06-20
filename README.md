# fraunhofer-devops-day-2024

LaTeX Beamer slides from my talk at **Fraunhofer DevOps Day 2024** (August 13, 2024).

## About

This talk demonstrates a one-click, on-demand Kubernetes cluster rollout using
**GitLab CI/CD**, **Terraform**, **Argo CD** and **Rancher**. The architecture
follows DevOps best practices — infrastructure as code, GitOps for bootstrapping,
and a fully automated pipeline as a reusable CI/CD component.

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
```

### Build

```bash
latexmk -pdf CICD_Rollouts_auf_Rancher_mit_Terraform.tex
```

### Clean

```bash
latexmk -c
```
