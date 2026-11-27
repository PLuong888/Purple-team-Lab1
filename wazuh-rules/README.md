# Wazuh rules: source configuration not yet supplied

The user-provided PDF contains screenshots of the `local_rules.xml` editor and of rule `100002` in the Wazuh Dashboard, but does not provide a verified original XML file. **Do not publish a fabricated or untested rule** as an operational configuration.

Export the real `/var/ossec/etc/rules/local_rules.xml` from the Wazuh Manager, review its matches and MITRE mapping, test it with representative logs using `wazuh-logtest`, then place a sanitised copy here.
