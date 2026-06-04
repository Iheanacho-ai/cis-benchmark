====================================================================================================
# 5.3.1  —  Configure Control Plane Firewall
====================================================================================================

## [section #]
5.3.1

## [title]
Configure Control Plane Firewall

## [overview]
The Kubernetes control plane nodes run essential services for both Kubernetes and Talos Linux cluster management, and as such should be protected from unauthorized network traffic. The following rules improve the security of the cluster and cover only standard Kubernetes and Talos Linux services. If additional services are running with host networking in the cluster, they should be covered by additional rules.
