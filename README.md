# Bitbucket Server and Jenkins

This is a demo of using Bitbucket Server and Jenkins to perform releases by pushing tags to Git.

There is a sample payload of a tag being pushed in `tag-sample-payload.json`.

There is a sample build log in `build-log-sample.txt`.

## Setup

See `Jenkinsfile` for the script performing the release.

Let the repository in Bitbucket Server have a webhook pushing tag events to: `http://jenkins:8080/generic-webhook-trigger/invoke?token=abc123`

## Usage

Start it with `docker-compose up` and you will get:

 - Bitbucket Server: http://localhost:7990/
 - Jenkins: http://localhost:8080/
