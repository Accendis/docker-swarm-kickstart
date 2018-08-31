# Docker Swarm Kickstart

> A initial Docker Swarm template to build with monitoring, logs and tracing.

## Introduction

Many companies have trouble setting a correct, visible and auditable infrastructure with Docker. This project comes as a starting point to build reliable microservice architecture with full visibility from the ground up.

## What's in the package

1. To handle logs we use ELK (ElasticSearch, Logstash, Kibana).
2. To handle tracing, we use OpenZipkin.
3. To handle errors and exception notification, we use Sentry (On Premise).
4. (Optional) To have a full visual of the Docker Cluster, we use Swarmpit.

## Installing everything in the cluster.

### Step 0 - Configure Docker Volume Driver

Volume drivers are a way to store outside a node, in a remote filesystem, the persistent data of a container. We recommend using a volume driver instead of local one.

### Step 1 - Install ELK Stack, to capture logs.

Logging is one of the most important parts of any infrastructure. We start by installing an ELK stack, that we will use to redirect all logging from other stacks to it.

### Step 1.5 [Optional] - Install Swarmpit

Swarmpit helps us on managing a docker swarm cluster. This might be the prefered option for some people, while some people may dislike it. Personally, I find easier to handle deployments and such with a tool like Swarmpit.

