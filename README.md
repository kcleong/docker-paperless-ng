# Paperless-ng docker config

Docker-compose configuration to set-up 
[Paperless-ng](https://github.com/jonaswinkler/paperless-ng) with redis and \
[rclone](https://rclone.org).

Rclone is used to sync the scans on an cloud storage to Paperless.

## Getting started

    cp docker-compose.env.example docker-compose.env
	mkdir -p paperless/data
	mkdir -p paperless/media
	mkdir -p paperless/export
	mkdir -p paperless/consume
	mkdir rclone

Add rclone config file in `rclone/config` and configure rclone path in
`docker-compose.yml`.
