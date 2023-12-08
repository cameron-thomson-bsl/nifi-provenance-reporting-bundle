[![Build Status](https://github.com/brightsparklabs/nifi-provenance-reporting-bundle/actions/workflows/test.yml/badge.svg)](https://github.com/brightsparklabs/nifi-provenance-reporting-bundle/actions/workflows/test.yml)

# nifi-provenance-reporting-bundle

NiFi provenance reporting tasks.

## Table of Contents

- [Installation](#installation)
- [Tasks](#tasks)
    - [ElasticsearchProvenanceReporter](#elasticsearchprovenancereporter)
    - [HttpProvenanceReporter](#httpprovenancereporter)
- [Todo](#todo)
- [Publishing](#publishing)
- [License](#license)

## Installation

```sh
$ gradle nar
$ cp build/libs/nifi-provenance-reporting-nar-<version>.nar $NIFI_HOME/lib
$ nifi restart
```

## Tasks

### ElasticsearchProvenanceReporter

Reporting task to write provenance events to an Elasticsearch index.

#### Reporting Task Properties

<img src="elasticsearch_provenance_reporter_properties.png" width=600 />

#### Example Event

<img src="elasticsearch_provenance_reporter_event.png" width=600 />

### HttpProvenanceReporter

Reporting task to POST provenance events to an HTTP web service.

#### Reporting Task Properties

This reporting task can be configured to POST provenance events to an arbitrary web service. Here is an example of using it with Solr (10s commits):

<img src="http_provenance_reporter_properties.png" width=600 />

## Todo

- Add batching support.
- Additional adapters:
    - HDFS
    - Tinkerpop
    - NiFi site-to-site
- Optional inclusion of FlowFile contents.
- Create provenance event for runs of the reporting task.
- Example schemas/mappings for data sources (Elasticsearch mapping, Solr schema, JSON schema).
- Add testing.

## Publishing

```
# E.g. for version '1.99.2' (MUST START with '1.')
version=1.99.2

git checkout 1.x.x
git pull
git tag -a -m "<TICKET>: Tag version ${version}" ${version}
git push --tags
```

This will then be automatically published by the CI server.

## License

Copyright (c) 2023 brightSPARK Labs (from commit `477827d4818d475e23801006dc0e9273b70fd159`
onwards).

Copyright (c) 2016 Joey Frazee (to and including commit `477827d4818d475e23801006dc0e9273b70fd159`).

nifi-provenance-reporting-bundle is released under the Apache License Version 2.0.
