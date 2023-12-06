# "Howto use a SIEM system against CyberCrime"

This repo includes docs about a workshop from [DevOpenSpace 2023](https://devopenspace.de) course about [Wazuh](https://wazuh.com) security platform.

* [this document](./Readme.md)
* [todays plan](./workshop_overview.md)

## attached documents

* [example agent config](./agent.conf) to deploy from central server to all Wazuh agents
* [additional config file](./local_internal_options.conf) for agents to allow Wazuh server pushing centralized config
* [technical concept graphic](./technical_concept_draft.jpg) how to run build a security platform around Wazuh
* [Crontab file to cleanup logs](./wazuh_cleanup_crontab)
* [JSON file](./wazuh_index_policy.json) including index policy to cleanup alerts after X days
* [info graphic](./what_Wazuh_is_not.jpg) to tell what Wazuh can not do

## Links

* [Wazuh documentation](https://documentation.wazuh.com/current/getting-started/index.html) is actually good to work with
* [Wazuh blog](https://wazuh.com/blog/) describes a huge amount of solutions to cover certain security aspects
* [Wazuh community](https://wazuh.com/community/) helps a lot, for example Discord server
* [Wazuh rulesets on Github](https://github.com/wazuh/wazuh-ruleset) to see what runs out of the box
* [more helpful rules on Github](https://github.com/socfortress/Wazuh-Rules)
* [Shuffler.io automation software on Github](https://github.com/orgs/Shuffle/repositories)