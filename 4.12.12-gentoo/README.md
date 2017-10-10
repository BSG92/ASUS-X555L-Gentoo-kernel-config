# Gentoo kernel 4.12.12.
### FEATURES
- All ACPI/Hot keys are working. (Need to remove any "acpi_osi" and/or "acpi_backlight" directives in grub configuration for brightness keys to work).
- Changed "CONFIG_GENERIC_CPU=y" to "CONFIG_MCORE2=y".
- Changed "CONFIG_COMPAT_VDSO=y" to "CONFIG_COMPAT_VDSO=n" (Some glibc versions may find this buggy, change this at any time).
- Removed many unwanted soundcard drivers for a base system.
### TO-DO
- Airplane mode LED does not respond.
