---
tags: [facet, orbitdb, decentralized, crdt]
---

# OrbitDB Facet

## Overview

The OrbitDB Facet of PaperClip is designed to ensure reliable and scalable storage of knowledge artifacts using a decentralized, CRDT-based architecture. Each PaperClip node runs its own OrbitDB instance, providing distributed, peer-to-peer storage with eventual consistency and conflict-free data synchronization.

## Features

1. **Decentralized Database**: Each PaperClip node maintains its own OrbitDB, eliminating single points of failure.
2. **CRDT-Based Consistency**: Ensures eventual consistency and conflict-free data synchronization across nodes.
3. **Scalability**: Handles large datasets and concurrent access seamlessly across distributed PaperClip nodes.
4. **Extensibility**: Supports custom data models and advanced querying capabilities.
5. **Integration**: Easily integrates with other components of PaperClip.

## Node Setup

A typical deployment consists of three PaperClip nodes, each running its own OrbitDB instance. These nodes are managed via a custom ALM (Automated Lifecycle Management) charm developed as part of the Witchcraft project.

- The charm automates the deployment and management of the three PaperClip nodes.
- Each node participates equally in data storage and synchronization.
- The system is resilient to individual node failures due to its decentralized nature.

### Custom ALM Charm

The custom ALM charm for PaperClip nodes will be developed as part of the Witchcraft project. You can find the repository here:  
[Rainfall-One/Crucible](https://github.com/rainfall-one/crucible)

### Deployment Example

Below is an example of deploying a three-node PaperClip cluster (each with OrbitDB) with the custom ALM charm:

```bash
juju deploy paperclip --num-units=3 --channel=edge
juju deploy alm-charm --config monitoring=true
juju relate paperclip alm-charm
```


## Diagram

<div align="center">

<pre>
       +-------------------+
                  |     PaperClip     |  (x3 nodes)
       +-------------------+
       |                   |
       |   OrbitDB Local   |
       |                   |
       +-------------------+
       |                   |
       |   ALM Features    |
       |                   |
       +-------------------+
       |                   |
       |   Custom Charm    |
       |                   |
       +-------------------+
</pre>

</div>
