# Ixcoin for Docker

[![Build Status](https://travis-ci.org/acejam/docker-ixcoin.svg?branch=master)](https://travis-ci.org/acejam/docker-ixcoin)
[![Docker Stars](https://img.shields.io/docker/stars/acejam/ixcoin.svg?maxAge=2592000)](https://hub.docker.com/r/acejam/ixcoin)
[![Docker Pulls](https://img.shields.io/docker/pulls/acejam/ixcoin.svg?maxAge=2592000)](https://hub.docker.com/r/acejam/ixcoin)

A customizable Docker container for Ixcoin

## Quick Start

    docker run -d --name ixcoin --restart=always -v /data/ixcoin:/data/ixcoin acejam/ixcoin:latest

## Config options

This container includes support for Ixcoin configuration values. These values can be set when calling `docker run` through the use of environment variables.

The following values are configurable:
* `RPC_USER`
* `RPC_PASS`
* `RPC_ALLOW_IP`
* `MAX_CONNECTIONS`
* `RPC_PORT`
* `PORT`

For example, to run the container with the username "DevUser" and a password of "P@ssw0rd123" with 10 max connections, you can run the following:

      docker run -d -e RPC_USER="DevUser" -e RPC_PASS="P@ssw0rd123" -e MAX_CONNECTIONS=10 acejam/ixcoin:latest

## Data persistence

Coming soon!
