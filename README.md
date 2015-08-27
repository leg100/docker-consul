

## Containers for Hashicorp's Consul

Includes a `docker-compose.yml` for running a 3-node consul server cluster.

Uses Ubuntu as a base image. Other containers run on alpine-linux to reduce file size. But I found an issue whereby hostnames are not looked up in /etc/hosts. This prevents docker links from working, which docker-compose relies upon. 

### leg100/consul [![](https://badge.imagelayers.io/leg100/consul:latest.svg)](https://imagelayers.io/?images=leg100/consul:latest 'Get your own badge on imagelayers.io')
Barebones, no configuration files included

### leg100/consul-agent [![](https://badge.imagelayers.io/leg100/consul-agent:latest.svg)](https://imagelayers.io/?images=leg100/consul-agent:latest 'Get your own badge on imagelayers.io')
Configured to run as an agent

### leg100/consul-server [![](https://badge.imagelayers.io/leg100/consul-server:latest.svg)](https://imagelayers.io/?images=leg100/consul-server:latest 'Get your own badge on imagelayers.io')  
Configured to run as a server, includes UI


