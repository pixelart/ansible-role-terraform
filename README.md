# Ansible Role: Terraform

[![Build Status](https://travis-ci.org/pixelart/ansible-role-terraform.svg?branch=master)](https://travis-ci.org/pixelart/ansible-role-terraform)

Installs [Hashicorp's Terraform](https://www.terraform.io/).

## Requirements

  - `unzip` package must be installed to extract the download.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    terraform_version: '0.9.5'

The version of Terraform which should be installed.

    terraform_install_path: '/usr/local/bin'

The path where the Terraform binary should be installed. Ensure it's in your `$PATH`.

## Dependencies

None.

## Example Playbook

    - hosts: all
      roles:
        - pixelart.terraform

After the playbook runs, `terraform` will be accessible via normal user accounts.

## Code of Conduct

Please note that this project is released with a [Contributor Code of Conduct](CODE_OF_CONDUCT.md). By participating in this project you agree to abide by its terms.

## License

MIT, see the [LICENSE](LICENSE) file.

## Author Information

This role was created in 2017 by [pixelart GmbH](https://www.pixelart.at/).
