# kubernetes-cluster-architecture.
Documentation on Kubernetes Cluster Architecture
# Kubernetes Cluster Architecture

This repository provides an overview of the architectural concepts behind Kubernetes. A Kubernetes cluster consists of a control plane and a set of worker nodes that run containerized applications.

## Key Concepts

- **Control Plane**: Manages the worker nodes and Pods in the cluster.
- **Worker Nodes**: Host the Pods that comprise the application workload.

## Components

- [Control Plane Components](components/control_plane.md)
- [Node Components](components/node_components.md)
- [Addons](components/addons.md)
- [Architecture Variations](components/architecture_variations.md)


# Control Plane Components

The control plane makes decisions about the cluster.

## Key Components
- **kube-apiserver**: Exposes the Kubernetes API.
- **etcd**: Key-value store for cluster data.
- **kube-scheduler**: Assigns Pods to nodes.
- **kube-controller-manager**: Manages controllers.
- **cloud-controller-manager**: Links to cloud provider APIs.


# Node Components

These components run on every node.

## Key Components
- **kubelet**: Ensures containers are running in Pods.
- **kube-proxy**: Manages network rules.
- **Container Runtime**: Manages containers' lifecycle.


# Addons

Addons enhance cluster features.

## Key Addons
- **DNS**: For service discovery.
- **Web UI (Dashboard)**: Interface for managing applications.


# Architecture Variations

Different deployment options exist.

## Control Plane Deployment Options
- **Traditional**: Runs on dedicated machines.
- **Static Pods**: Managed by the kubelet.
