# Gitlab-CE updater

This project focus on updating the GitLab CE (Community Edition).
Main reason for updating script is because system update usualy skip minor version and gitlab unable to run because of lack of migration process.

At this moment updating scipt focus on apt based distribution.

## Logical steps

1. List available versions.
2. Get intalled version.
3. Update package to incremental version.
4. gitlab recofigure
5. gitlab db migrate
6. Hold package version in package manager to prevent updates

## Ideas to implement

* control versions over Ansible to make it easier to manage multiple Linux distribution.
* Python script for upgrading process
