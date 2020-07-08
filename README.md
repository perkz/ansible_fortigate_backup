# ansible_fortigate_backup

Fortigate devices have a reasonably good set of Ansible modules for configuring devices that uses the REST API, however one thing that is missing is the ability to pull the config from a device.

This has been possible in the past using the fortios_config ansible module, however that relies on pyFG which unfortunately appears to be unmaintained and can be difficult to get working reliably.

This Ansible runbook shows an example of how to pull the config from a Fortigate using session-based authentication via the REST API and save it to a local GIT repo.

You could modify this to also use token-based authentication. For more information, see here: https://kb.fortinet.com/kb/documentLink.do?externalID=FD45595
