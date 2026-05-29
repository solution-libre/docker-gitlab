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
with [Traefik] by [Solution Libre].

## Setup

```sh
cd /opt
git clone https://usine.solution-libre.fr/docker/gitlab.git gitlab
cd gitlab
```

Declare environment variables or copy the `.env.dist` to `.env` and adjust its values.

## Usage

```sh
cd /opt/gitlab
docker compose up -d
```

## Optional Integrations

This setup includes pre-configured labels for optional integrations with Traefik and Ofelia.
You can use them, customize them, or remove them based on your needs.

### Traefik (Reverse Proxy)

The Docker Compose files include [Traefik] labels for automatic HTTPS routing and SSL certificate management.
This is **optional** and recommended for production deployments.

**To use Traefik:**

The labels are already configured in the compose files for GitLab, Mattermost, and the Container Registry.
See [Solution Libre's Traefik setup](https://usine.solution-libre.fr/docker/traefik)
for a complete Traefik configuration compatible with this project.

### Ofelia (Scheduled Backups)

The `web` service includes Ofelia labels to automatically schedule GitLab backups every day at midnight.
This is **optional** and requires [Ofelia](https://github.com/mcuadros/ofelia) running on your Docker host.

**Current schedule:** Daily at 00:00 (midnight)

## Reference

See [REFERENCE.md](./REFERENCE.md).

## Development

[Solution Libre]'s repositories are open projects,
and community contributions are essential for keeping them great.

[Fork this repo on our GitLab](https://usine.solution-libre.fr/docker/gitlab/-/forks/new) or
[on GitHub](https://github.com/solution-libre/docker-gitlab/fork)

## Contributors

The list of contributors can be found at: <https://usine.solution-libre.fr/docker/gitlab/-/graphs/main>

[Solution Libre]: https://www.solution-libre.fr
[Traefik]: https://traefik.io/traefik
