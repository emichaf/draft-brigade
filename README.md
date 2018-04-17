# Draft Packs for Brigade

This project contains Draft packs oriented toward Brigade.

Available Packs:

- brigade-gateway: Quickly create a new Brigade gateway using a base Node.js project.

## Installation

Add this GitHub repo as a pack repository:

```console
$ draft pack-repo add https://github.com/technosophos/draft-brigade
```

You can verify that the repository was added using `draft pack-repo list`.

## Brigade-Gateway

Use the `brigade-gateway` pack to rapidly create custom Brigade webhook gateways. You can get a basic Brigade gateway running in under 5 minutes using this JavaScript builder.

To begin using Brigade gateway scaffold, simply do this:

```console
$ mkdir myGateway
$ cd myGateway
$ draft create --pack brigade-gateway
$ # Edit index.js
$ draft up
$ # See your work in progress:
$ draft connect
$ curl $URL_FROM_CONNECT/healthz
```

The `index.js` file is pre-configured for rapidly creating an HTTP/HTTPS Brigade gateway. Inside of the `index.js` file, you will find instructions for modifying it to suit your needs.

## Node Starter

The `node` starter pack is an opinionated Node.js application. It has two purposes:

1. Help Node.js developers get a running Kubernetes app in **less than two minutes**
2. Serve as a pattern for other deep language packs

To get started:

```
$ mkdir node-demo
$ cd node-demo

```
