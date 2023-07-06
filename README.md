# openstack-exporter

[![Source Code](https://img.shields.io/badge/github-source%20code-blue?logo=github&amp;logoColor=white)](https://github.com/rolehippie/openstack-exporter)
[![General Workflow](https://github.com/rolehippie/openstack-exporter/actions/workflows/general.yml/badge.svg)](https://github.com/rolehippie/openstack-exporter/actions/workflows/general.yml)
[![Readme Workflow](https://github.com/rolehippie/openstack-exporter/actions/workflows/readme.yml/badge.svg)](https://github.com/rolehippie/openstack-exporter/actions/workflows/readme.yml)
[![Galaxy Workflow](https://github.com/rolehippie/openstack-exporter/actions/workflows/galaxy.yml/badge.svg)](https://github.com/rolehippie/openstack-exporter/actions/workflows/galaxy.yml)
[![License: Apache-2.0](https://img.shields.io/github/license/rolehippie/openstack-exporter)](https://github.com/rolehippie/openstack-exporter/blob/master/LICENSE)
[![Ansible Role](https://img.shields.io/badge/role-rolehippie.openstack__exporter-blue)](https://galaxy.ansible.com/rolehippie/openstack_exporter)

Ansible role to install and configure a Prometheus exporter for OpenStack.

## Sponsor

Building and improving this Ansible role have been sponsored by my current and previous employers like **[Cloudpunks GmbH](https://cloudpunks.de)** and **[Proact Deutschland GmbH](https://www.proact.eu)**.

## Table of content

- [Requirements](#requirements)
- [Default Variables](#default-variables)
  - [openstack_exporter_admin_password](#openstack_exporter_admin_password)
  - [openstack_exporter_admin_username](#openstack_exporter_admin_username)
  - [openstack_exporter_api_version](#openstack_exporter_api_version)
  - [openstack_exporter_auth_url](#openstack_exporter_auth_url)
  - [openstack_exporter_auth_verify](#openstack_exporter_auth_verify)
  - [openstack_exporter_identity_interface](#openstack_exporter_identity_interface)
  - [openstack_exporter_image](#openstack_exporter_image)
  - [openstack_exporter_network](#openstack_exporter_network)
  - [openstack_exporter_project_domain](#openstack_exporter_project_domain)
  - [openstack_exporter_project_name](#openstack_exporter_project_name)
  - [openstack_exporter_publish](#openstack_exporter_publish)
  - [openstack_exporter_pull_image](#openstack_exporter_pull_image)
  - [openstack_exporter_region_name](#openstack_exporter_region_name)
  - [openstack_exporter_user_domain](#openstack_exporter_user_domain)
  - [openstack_exporter_version](#openstack_exporter_version)
- [Discovered Tags](#discovered-tags)
- [Dependencies](#dependencies)
- [License](#license)
- [Author](#author)

---

## Requirements

- Minimum Ansible version: `2.10`


## Default Variables

### openstack_exporter_admin_password

Password to authenticate on OpenStack

#### Default value

```YAML
openstack_exporter_admin_password:
```

### openstack_exporter_admin_username

Username to authenticate on OpenStack

#### Default value

```YAML
openstack_exporter_admin_username:
```

### openstack_exporter_api_version

Version of the OpenStack identity API

#### Default value

```YAML
openstack_exporter_api_version: 3
```

### openstack_exporter_auth_url

URL to access the OpenStack identity API

#### Default value

```YAML
openstack_exporter_auth_url:
```

### openstack_exporter_auth_verify

Verify the SSL certificate

#### Default value

```YAML
openstack_exporter_auth_verify: true
```

### openstack_exporter_identity_interface

Interface of the OpenStack identity API

#### Default value

```YAML
openstack_exporter_identity_interface: public
```

### openstack_exporter_image

Docker image to use and run

#### Default value

```YAML
openstack_exporter_image: ghcr.io/openstack-exporter/openstack-exporter:{{ openstack_exporter_version
  }}
```

### openstack_exporter_network

A Docker network to assign the container

#### Default value

```YAML
openstack_exporter_network:
```

### openstack_exporter_project_domain

Domain of the project

#### Default value

```YAML
openstack_exporter_project_domain: Default
```

### openstack_exporter_project_name

Name of the project

#### Default value

```YAML
openstack_exporter_project_name: admin
```

### openstack_exporter_publish

Publish the Docker image on thet binding

#### Default value

```YAML
openstack_exporter_publish: 9180
```

### openstack_exporter_pull_image

Pull image as part of the tasks

#### Default value

```YAML
openstack_exporter_pull_image: true
```

### openstack_exporter_region_name

Name of the OpenStack region

#### Default value

```YAML
openstack_exporter_region_name: RegionOne
```

### openstack_exporter_user_domain

Domain of the users

#### Default value

```YAML
openstack_exporter_user_domain: Default
```

### openstack_exporter_version

Version of the Docker image

#### Default value

```YAML
openstack_exporter_version: 1.6.0
```

## Discovered Tags

**_openstack-exporter_**


## Dependencies

- [rolehippie.docker](https://github.com/rolehippie/docker)

## License

Apache-2.0

## Author

[Thomas Boerger](https://github.com/tboerger)
