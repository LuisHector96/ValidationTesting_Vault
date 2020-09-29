To play with this repo:
- Need to add vars for [group vars](group_vars/all.yml)
- Need to add your AWS Credentials


How to run playbook?

Command:

'''
    ansible-playbook validate_vault.yml -i inventory.yml
'''

Validation Testing Framework for vaultVault built in ansible.

Checks API entrypoints for Status 200 on:
- Init
- Seal
- Tokens
- Metrics
- Audit

New Features Added:
- Show No. of Consul and Vault nodes
- Consul UI status (pass if Disabled)
- Checking Status of Splunk and Qualys
- Checking Vault Oracle plugin version

A tester and a telemetry policies should be added first with a token, or use root token for the requests but that is not recommended.
