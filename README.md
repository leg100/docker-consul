[![](https://badge.imagelayers.io/leg100/consul:latest.svg)](https://imagelayers.io/?images=leg100/consul:latest 'Get your own badge on imagelayers.io')

## Containers for Hashicorp's Consul

* leg100/consul - barebones, no configuration files included
* leg100/consul-agent - configured to run as an agent
* leg100/consul-server - configured to run as a server, includes UI

Includes a `docker-compose.yml` for running a 3-node consul server cluster.

Uses Ubuntu as a base image. Other containers run on alpine-linux to reduce file size. But I found an issue whereby hostnames are not looked up in /etc/hosts. This is a problem when relying on docker links, which adds entries to /etc/hosts.
