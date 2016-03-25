---
layout: documentation
title: Documentation
skip_title: true
---

[Transitland](https://transit.land) brings together many sources of transit data to build a [directory of operators and feeds](https://transit.land/feed-registry/) that can be edited by transit enthusiasts and developers.

![a diagram showing the Transitland Feed Registry, Datastore, and Playground communicating with each other](/images/how-it-works-diagram.png)

Transitland Feed Registry is a directory of public-transit operators and their authoritative data feeds. The directory is a view into Transitland's Datastore API. It lets users browse operators and their feeds, as well as view the license restrictions on each feed and contribute additional operators and feeds.

Transitland Datastore brings together data from authoritative sources (listed in the Feed Registry) with contributions, edits, and fixes from transit enthusiasts and developers. It's a hosted service that provides a simple web API for query and editing.

Onestop ID: With data coming from many different sources, we've had to fashion some glue link together stops, routes, and schedules across operators. Onestop is Transitland's experimental attempt to build a stable, globally unique identifier scheme. The Datastore API returns Onestop IDs for every feed, operator, stop, and route.

Transitland Dispatcher: We use an administrative interface to review submissions and monitor feed aggregation. Anyone else can peek in and see what's happening inside the Transitland Datastore.

Transitland Playground demonstrates all the pieces of the data architecture working together.

All of Transitland's software components are available under open-source licenses; all of the data (federated from authoritative sources and contributed by community members) is freely available. You can participate in Transitland by using just one component of this architecture, or come for it all.
