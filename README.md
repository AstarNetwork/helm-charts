# universal-helm

This repository contains the `universal-helm` Helm chart, which can generate Kubernetes manifests to deploy and expose a blockchain node using Ingress.

## Motivation to Use a Common Helm Chart for All Blockchain Nodes

**Pros:**
  - **More DRY Infra as Code:** All blockchain nodes share a significant amount of configuration, which is generalized in this Helm chart.
  - **Easier Infra as Code Development:** Using the same Helm chart for all nodes allows changes to be made in one place to bring new features or fix bugs for all nodes.
  - **Unified Code and Naming Conventions:** All nodes follow the same code and naming conventions specified in the Helm chart, resulting in a more uniform infrastructure that is easier to read and develop.

**Cons:**
  - **Increased Configuration Items:** Due to generalization, nodes' configurations include more items, resulting in more lines of code.

## Structure of the Repository

The Helm chart includes templates for the following objects:
  - **StatefulSets:** Deploys blockchain node containers. Init containers can be used to download snapshots, initialize data, etc. It will also automatically add a sidecar container with health probes to check the node's status.
  - **Services:** Generated for each [container's port]().
  - **Ingresses:** Exposes ports to the outside world; see [example]().

Example node configurations can be found in examples folder.

[Repo index](./index.yaml)
