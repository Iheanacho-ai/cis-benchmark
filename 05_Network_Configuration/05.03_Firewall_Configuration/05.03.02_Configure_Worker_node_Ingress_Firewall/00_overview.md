====================================================================================================
# 5.3.2  —  Configure Worker node Ingress Firewall
====================================================================================================

## [section #]
5.3.2

## [title]
Configure Worker node Ingress Firewall

## [overview]
The Kubernetes worker nodes should be protected from unauthorized network traffic in order to protect the services running on them, and the cluster itself. The following rules improve the security of the cluster and cover only standard Kubernetes and Talos Linux services. If additional services are running with host networking in the cluster, they should be covered by additional rules.
