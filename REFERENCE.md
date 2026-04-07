# Reference

## Environment variables

| Name                               | Description                                                                 | Default value                  |
| ---------------------------------- | --------------------------------------------------------------------------- | ------------------------------ |
| `DOMAIN`                           | The root domain                                                             | `domain.tld`                   |
| `GITLAB_SUBDOMAIN`                 | The GitLab subdomain                                                        | `gitlab`                       |
| `GITLAB_SSH_PORT`                  | The GitLab SSH port for git                                                 | `22`                           |
| `GITLAB_VERSION`                   | The GitLab image version                                                    | `18.10.1`                      |
| `GITLAB_RUNNER_VERSION`            | The GitLab Runner image version                                             | `18.10.0`                      |
| `MATTERMOST_ENABLE`                | To enable Mattermost set `true`. To disable Mattermost leave empty.         |                                |
| `MATTERMOST_SUBDOMAIN`             | The Mattermost subdomain                                                    | `mattermost`                   |
| `NGINX_REAL_IP_TRUSTED_ADDRESSES`  | List of trusted addresses for the real IP header                            | `[]`                           |
| `OBJECT_STORAGE_ENABLE`            | To enable Object Storage set `true`. To disable Object Storage leave empty. |                                |
| `OBJECT_STORAGE_ACCESS_KEY`        | The Object Storage access key                                               | `s3-access-key`                |
| `OBJECT_STORAGE_BUCKET_PREFIX`     | The Object Storage bucket prefix                                            | `your-s3-bucket-prefix-`       |
| `OBJECT_STORAGE_ENDPOINT`          | The Object Storage endpoint URL                                             | `https://s3.domain.tld`        |
| `OBJECT_STORAGE_REGION`            | The Object Storage region                                                   | `your-s3-region`               |
| `OBJECT_STORAGE_SECRET_KEY`        | The Object Storage secret key                                               | `s3-secret-key`                |
| `REGISTRY_ENABLE`                  | To enable Registry set `true`. To disable Registry leave empty.             |                                |
| `REGISTRY_SUBDOMAIN`               | The Registry subdomain                                                      | `registry`                     |
| `REGISTRY_STORAGE_ACCESS_KEY`      | The Registry S3 access key                                                  | `${OBJECT_STORAGE_ACCESS_KEY}` |
| `REGISTRY_STORAGE_BUCKET`          | The Registry S3 bucket                                                      | `your-s3-bucket`               |
| `REGISTRY_STORAGE_REGION`          | The Registry S3 region                                                      | `${OBJECT_STORAGE_REGION}`     |
| `REGISTRY_STORAGE_REGION_ENDPOINT` | The Registry S3 region endpoint                                             | `${OBJECT_STORAGE_ENDPOINT}`   |
| `REGISTRY_STORAGE_SECRET_KEY`      | The Registry S3 secret key                                                  | `${OBJECT_STORAGE_SECRET_KEY}` |
| `SMTP_ENABLE`                      | To enable SMTP set `true`. To disable SMTP leave empty.                     |                                |
| `SMTP_ADDRESS`                     | The SMTP server address                                                     | `smtp.domain.tld`              |
| `SMTP_DOMAIN`                      | The SMTP domain                                                             | `my.domain.tld`                |
| `SMTP_ENABLE_STARTTLS_AUTO`        | Whether to enable STARTTLS automatically                                    | `false`                        |
| `SMTP_PORT`                        | The SMTP server port                                                        | `465`                          |
| `SMTP_TLS`                         | Whether to use TLS for SMTP                                                 | `true`                         |
| `SMTP_USER_NAME`                   | The SMTP username                                                           | `my-smtp-user`                 |
| `SMTP_USER_PASSWORD`               | The SMTP password                                                           | `my-smtp-password`             |
