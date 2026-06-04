====================================================================================================
# 1.1  —  Boot Settings
====================================================================================================

## [section #]
1.1

## [title]
Boot Settings

## [overview]
The recommendations in this section focus on securing the bootloader and settings involved in the boot process directly.
Talos supports booting UEFI systems in SecureBoot mode. When combined with TPM-based disk encryption, this provides Trusted Boot, which extends protection to *initrd*, and a fully signed execution path from firmware to userspace.
