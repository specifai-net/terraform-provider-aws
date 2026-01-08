<!-- Copyright IBM Corp. 2014, 2025 -->
<!-- SPDX-License-Identifier: MPL-2.0 -->

<!-- markdownlint-disable first-line-h1 no-inline-html -->
<a href="https://terraform.io">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset=".github/terraform_logo_dark.svg">
    <source media="(prefers-color-scheme: light)" srcset=".github/terraform_logo_light.svg">
    <img src=".github/terraform_logo_light.svg" alt="Terraform logo" title="Terraform" align="right" height="50">
  </picture>
</a>

# Terraform AWS Provider

[![Forums][discuss-badge]][discuss]

[discuss-badge]: https://img.shields.io/badge/discuss-terraform--aws-623CE4.svg?style=flat
[discuss]: https://discuss.hashicorp.com/c/terraform-providers/tf-aws/

The [AWS Provider](https://registry.terraform.io/providers/hashicorp/aws/latest/docs) enables [Terraform](https://terraform.io) to manage [AWS](https://aws.amazon.com) resources.

- [Contributing guide](https://hashicorp.github.io/terraform-provider-aws/)
- [Quarterly development roadmap](ROADMAP.md)
- [FAQ](https://hashicorp.github.io/terraform-provider-aws/faq/)
- [Tutorials](https://learn.hashicorp.com/collections/terraform/aws-get-started)
- [discuss.hashicorp.com](https://discuss.hashicorp.com/c/terraform-providers/tf-aws/)

_**Please note:** We take Terraform's security and our users' trust very seriously. If you believe you have found a security issue in the Terraform AWS Provider, please responsibly disclose it by contacting us at security@hashicorp.com._

### HOW TO BUILD (SpecifAI)
To make a release, follow the next steps:
- Install goreleaser locally
- Run the following command:
```
GITHUB_TOKEN=<GITHUB_TOKEN> GPG_FINGERPRINT=<FINGERPRINT> GPG_TTY=$(tty) goreleaser --clean
```

Where GITHUB_TOKEN can be found in the secrets repo and GPG_FINGERPRINT is the ID of the GPG_SECRET_KEY