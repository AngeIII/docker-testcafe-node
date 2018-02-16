# docker-testcafe-node

NOTE: Use for testing only! Root user is being used. Currently using it for running
end to end tests in CircleCI.

To implement, your script should run the following in the container:

`/opt/testcafe/bin/testcafe-with-v8-flag-filter.js 'chromium:headless --no-sandbox' <test directory>`

https://github.com/theogravity/docker-testcafe-node

https://hub.docker.com/r/personalife/docker-testcafe-node

- Docker-in-docker
- Alpine linux
- Alpine chrome
- curl
- python + pip
- awscli
- bash
- jq
- ecs-deploy
- boto3
- yarn

## Publishing

This repo is integrated directly into docker cloud for auto-publishing.

- When a PR goes into master, a new docker image tagged with `latest` is automatically created
- When A new version is tagged under github releases, a
new docker image will be created with that tag. The tag version format must be `vX.Y.Z`
