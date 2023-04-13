---
title: "Image Overview: prometheus-elasticsearch-exporter"
type: "article"
description: "Overview: prometheus-elasticsearch-exporter Chainguard Images"
date: 2022-11-01T11:07:52+02:00
lastmod: 2022-11-01T11:07:52+02:00
draft: false
tags: ["Reference", "Chainguard Images", "Product"]
images: []
menu:
  docs:
    parent: "images-reference"
weight: 500
toc: true
---

`experimental` [cgr.dev/chainguard/prometheus-elasticsearch-exporter](https://github.com/chainguard-images/images/tree/main/images/prometheus-elasticsearch-exporter)
| Tags     | Aliases                         |
|----------|---------------------------------|
| `latest` | `1`, `1.5`, `1.5.0`, `1.5.0-r1` |



Minimal Prometheus Image

## Get It!

The image is available on `cgr.dev`:

```
docker pull cgr.dev/chainguard/prometheus-elasticsearch-exporter:latest
```

## Usage

This image is a drop-in replacement for the upstream image.
For full configuration, see the [documentation there](https://github.com/prometheus-community/elasticsearch_exporter).

To test:

```shell
$ docker run cgr.dev/chainguard/prometheus-elasticsearch-exporter
level=info ts=2023-03-31T23:08:40.120364051Z caller=clusterinfo.go:214 msg="triggering initial cluster info call"
level=info ts=2023-03-31T23:08:40.120446635Z caller=clusterinfo.go:183 msg="providing consumers with updated cluster info label"
level=error ts=2023-03-31T23:08:40.121301718Z caller=clusterinfo.go:267 msg="failed to get cluster info" err="Get \"http://localhost:9200/\": dial tcp 127.0.0.1:9200: connect: connection refused"
level=error ts=2023-03-31T23:08:40.121330676Z caller=clusterinfo.go:188 msg="failed to retrieve cluster info from ES" err="Get \"http://localhost:9200/\": dial tcp 127.0.0.1:9200: connect: connection refused"
```

