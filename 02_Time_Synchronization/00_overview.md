====================================================================================================
# 2  —  Time Synchronization
====================================================================================================

## [section #]
2

## [title]
Time Synchronization

## [overview]
It is recommended that physical systems and virtual guests lacking direct access to the physical host's clock be configured to synchronize their time using NTP. Talos Linux has integrated support for NTP in the machined daemon, that is part of every Talos Linux install. Thus the recommendation is to ensure NTP is configured and operating correctly.
