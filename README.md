# GitLab with Docker Compose

<!-- markdownlint-disable-next-line MD001 -->
#### Table of Contents

1. [Description](#description)
2. [Setup](#setup)
3. [Usage](#usage)
4. [Reference](#reference)
5. [Development](#development)
6. [Contributors](#contributors)

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
docker-compose up -d
```

## Reference

### Environment variables

#### `GITLAB_HOSTNAME`

The GitLab hostname. Default value: 'my.domain.tld'

#### `GITLAB_SSH_PORT`

The GitLab SSH port for git. Default value: '22'

## Development

[Solution Libre](https://www.solution-libre.fr)'s repositories are open projects,
and community contributions are essential for keeping them great.

[Fork this repo on GitHub](https://github.com/solution-libre/docker-gitlab/fork)

## Contributors

The list of contributors can be found at: <https://github.com/solution-libre/docker-gitlab/graphs/contributors>
