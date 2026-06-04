====================================================================================================
# 3  —  Kubernetes
====================================================================================================

## [section #]
3

## [title]
Kubernetes

## [overview]
Talos Linux will install default vanilla Kubernetes, with many of the CIS Kubernetes benchmark recommendations applied by default. It is recommended that the CIS Kubernetes benchmark application be validated for any sensitive installation.
Specific further controls implemented or recommended by Talos Linux are below:

- Control plane scheduling: restrict workloads on control plane nodes.
- Pod Security Standards: set the Restricted policy, which is aimed at enforcing current Pod hardening best practices.
