====================================================================================================
# 6.2  —  Configure Service Logging
====================================================================================================

## [section #]
6.2

## [title]
Configure Service Logging

## [overview]
Logging services should be configured to prevent information leaks and to aggregate logs on a remote server so that they can be reviewed in the event of a system compromise and ease log analysis.

Talos Linux keeps recent logs in a ring buffer. The use of a ring buffer prevents the possibility of logs consuming all storage space and impacting system operation, but means that historical log events can be overwritten from the local system. It is strongly recommended that all logs are sent to a remote server. Talos Linux provides direct support for shipping these logs to a remote server.
