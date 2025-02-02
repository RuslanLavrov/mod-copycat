# mod-copycat

Copyright (C) 2020-2022 The Open Library Foundation

This software is distributed under the terms of the Apache License,
Version 2.0. See the file "[LICENSE](LICENSE)" for more information.

## Introduction

[mod-copycat](https://github.com/folio-org/mod-copycat) is a FOLIO  module
that assists in Copy cataloging. It can import records from remote systems
using Z39.50 or a straight MARC record can be provided.

mod-copycat provides two regular interface: `copycat-imports` and
`copycat-profiles`.

The provided interface `copycat-imports` is for the actual importing. There
are two modes:

1. raw record. The record is part of the import operation. The raw
record can be in JSON-MARC or as base64-encoded ISO2709.

2. Z39.50 search. The record is specified by a Z39.50 query and the
record is fetched and imported.

The interface `copycat-profiles` is a CRUD interface for managing copycat
profiles. These profiles include:

* job profiles - for the change manager.

* Z39.50 parameters.

## Additional information

Other FOLIO Developer documentation is at [dev.folio.org](https://dev.folio.org/)

### Issue tracker

See project [MODCPCT](https://issues.folio.org/browse/MODCPCT)
at the [FOLIO issue tracker](https://dev.folio.org/guidelines/issue-tracker).

### ModuleDescriptor

See the [ModuleDescriptor](descriptors/ModuleDescriptor-template.json)
for the interfaces that this module requires and provides, the permissions,
and the additional module metadata.

### Getting started

See [_Building, running, initializing and using mod-copycat_](doc/getting-started.md).

### API documentation

This module's [API documentation](https://dev.folio.org/reference/api/#mod-copycat).

### Code analysis

[SonarQube analysis](https://sonarcloud.io/dashboard?id=org.folio%3Amod-copycat).

### Download and configuration

The built artifacts for this module are available.
See [configuration](https://dev.folio.org/download/artifacts) for repository access,
and the [Docker image](https://hub.docker.com/r/folioorg/mod-copycat/).
