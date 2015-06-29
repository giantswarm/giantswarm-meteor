# Deploy a Meteor Application with Docker on Giant Swarm

This is a simple example of deploying Meteor applications with Docker on [Giant Swarm](https://giantswarm.io/).

Check out the full guide here:

https://blog.giantswarm.io/deploy-meteor-application-in-1-minute/

## Prerequisites

* A [Giant Swarm account](https://giantswarm.io/request-invite/) (or for local deployment [Docker](http://docs.docker.com/) and [Docker Compose](http://docs.docker.com/compose/install/))
* Your Meteor application in a GitHub repository (or somewhere else online)

## Deploying on the Swarm

1. Get the [swarm.json](https://github.com/giantswarm/giantswarm-meteor/blob/master/swarm.json) and save it to your local directory.
2. Edit the swarm.json to reflect your Meteor project’s GitHub URL* and desired domain.
3. `swarm up`
4. Profit

*: You can add an SSH-key or a custom (non-GitHub) Bundle-URL through the other environment variables detailed on the image’s [Docker Hub page](https://registry.hub.docker.com/u/ulexus/meteor/).
