====================================================================================================
# 5.1  —  Network Parameters (Host Only)
====================================================================================================

## [section #]
5.1

## [title]
Network Parameters (Host Only)

## [overview]
The following network parameters are intended for use if the system is to act as a host only. A system is considered host only if the system has a single interface, or has multiple interfaces but will not be configured as a router.

Because Kubernetes nodes generally have to act as routers in order to forward packets to the Pod subnets, it is unlikely that a Talos linux node will be configured as a Host Only.
