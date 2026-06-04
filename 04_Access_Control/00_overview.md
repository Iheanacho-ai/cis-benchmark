====================================================================================================
# 4  —  Access Control
====================================================================================================

## [section #]
4

## [title]
Access Control

## [overview]
Role Based Access in Talos<br>

Talos uses certificates to authorize users. The certificate subject’s organization field is used to encode user roles. There is a set of predefined roles that allow access to different API methods:<br>
- _os:admin_ grants access to all methods;
- _os:operator_ grants everything os:reader role does, plus additional methods: rebooting, shutting down, etcd backup, etcd alarm management, and so on;
- _os:reader_ grants access to “safe” methods (for example, that include the ability to list files, but do not include the ability to read file contents);
- _os:etcd:backup_ grants access to /machine.MachineService/EtcdSnapshot method.
Role Based Access Control is enabled for the Talos Linux API by default.

It is recommended that the least privileged access role that supports an administrator's required use be used.
