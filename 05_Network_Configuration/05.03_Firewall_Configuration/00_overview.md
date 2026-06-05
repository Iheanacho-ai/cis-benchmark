====================================================================================================
# 5.3  —  Firewall Configuration
====================================================================================================

## [section #]
5.3

## [title]
Firewall Configuration

## [overview]
The Talos Linux Ingress Firewall is a simple and effective way to limit network access to the services running on the host, which includes both Talos Linux and Kubernetes standard services (e.g. apid and kubelet), as well as any additional workload services that may be running on the host. The Talos Linux Ingress Firewall doesn’t affect the traffic between Kubernetes pods/services: please use CNI Network Policies for that.

In block mode, the ingress firewall will block encapsulated traffic (e.g. VXLAN) between cluster nodes. This traffic needs to be explicitly allowed for the Kubernetes networking to function properly. Please refer to the documentation for CNI in use for the required ports. See section 5.3.1.1 for an example of how to allow CNI encapsulated traffic.

Some default CNI configurations are listed below:

- Flannel, Calico: vxlan UDP port 4789
- Cilium: vxlan UDP port 8472

Note that traffic is always allowed on the following network interfaces:

- `lo`
- `siderolink`
- `kubespan`
