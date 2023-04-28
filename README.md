# GitLab with Docker Compose

<!-- markdownlint-disable-next-line MD001 -->
#### Table of Contents

- [GitLab with Docker Compose](#gitlab-with-docker-compose)
      - [Table of Contents](#table-of-contents)
  - [Description](#description)
  - [Setup](#setup)
  - [Usage](#usage)
  - [Reference](#reference)
    - [Environment variables](#environment-variables)
  - [Development](#development)
  - [Contributors](#contributors)

## Description

[Docker Compose](https://docs.docker.com/compose/) setup for starting [GitLab](https://gitlab.com/)
with [Træfik](https://traefik.io/).

## Setup

```sh
cd /opt
git clone https://github.com/solution-libre/docker-gitlab.git gitlab
cd gitlab
```

Declare environment variables or copy the `.env.dist` to `.env` and adjust its values.

## Usage

```sh
cd /opt/gitlab
docker compose up -d
```

## Reference

### Environment variables

| Name                               | Description                                                         | Default value                  |
| ---------------------------------- | ------------------------------------------------------------------- | ------------------------------ |
| `DOMAIN`                           | The GitLab domain                                                   | `domain.tld`                   |
| `GITLAB_SUBDOMAIN`                 | The GitLab subdomain                                                | `gitlab`                       |
| `GITLAB_SSH_PORT`                  | The GitLab SSH port for git.                                        | `22`                           |
| `MATTERMOST_ENABLE`                | To enable Mattermost set `true`. To disable Mattermost leave empty. |                                |
| `MATTERMOST_SUBDOMAIN`             | The Mattermost subdomain                                            | `mattermost`                   |
| `REGISTRY_ENABLE`                  | To enable Registry set `true`. To disable Registry leave empty.     |                                |
| `REGISTRY_SUBDOMAIN`               | The Mattermost subdomain                                            | `registry`                     |
| `REGISTRY_STORAGE_ACCESS_KEY`      | The S3 access key                                                   | `s3-access-key`                |
| `REGISTRY_STORAGE_BUCKET`          | The S3 bucket                                                       | `your-s3-bucket`               |
| `REGISTRY_STORAGE_REGION`          | The S3 region                                                       | `your-s3-region`               |
| `REGISTRY_STORAGE_REGION_ENDPOINT` | The S3 region endpoint                                              | `your-s3-regionendpoint`       |
| `REGISTRY_STORAGE_SECRET_KEY`      | The S3 secret key                                                   | `s3-secret-key-for-access-key` |
| `REGISTRY_SUBDOMAIN`               | The Registry subdomain                                              | `registry`                     |

## Development

[Solution Libre](https://www.solution-libre.fr)'s repositories are open projects,
and community contributions are essential for keeping them great.

[Fork this repo on GitHub](https://github.com/solution-libre/docker-gitlab/fork)

## Contributors

The list of contributors can be found at: <https://github.com/solution-libre/docker-gitlab/graphs/contributors>
