# DevOpenSpace workshop index

overview:

* 09:00
* 10:15 - 10:30 break
* 12:00 - 13:00 lunch break
* 14:30 coffee break
* 16:00 1000 questions, end

## introduction

* todays plan
* Who am I? Linkedin, DF, Platin Partner
* introduce Yourself
  - Who are You and what is Your job?
  - What do You want to learn today?
  - What do You know about SIEM and Wazuh so far?

## chapter 1: theory

* helpful web links
* What the SIEM?
  - What [problem](https://www.csoonline.com/de/a/diese-unternehmen-hat-s-schon-erwischt,3674038) do we want to solve?
  - Wtf is that? events, [SIEM, EDR, XDR, MDR, NDR](https://stripeolt.com/insights/cyber-security/cyber-security-jargon/)
  - What is it [not](./what_Wazuh_is_not.jpg)?
  - patch and update management
  - vulnerability scan vs. penetration testing
  - Wazuh as a "construction kit" for Your custom security platform
* Wazuh web interface
  - Agents and inventory
  - realtime event data, see one full log
  - dashboards & visalizations, embed filtered data tables
  - CVE scan
  - user management

## chapter 2: installation

* [Wazuh components overview](./technical_concept_draft.jpg)
* [installation server](https://documentation.wazuh.com/current/quickstart.html) (on Linux)
* [installation agent](https://documentation.wazuh.com/current/installation-guide/wazuh-agent/index.html) (on Windows)
* add sample data (through Wazuh settings page)
* confgure agents
  - [agent groups](https://documentation.wazuh.com/current/user-manual/agents/grouping-agents.html) (Management > Groups)
  - centralized agent configuration /var/ossec/etc/shared/
* server configuration
  - ossec.conf
  - remote syslog agents
    ```shell
    nc -u <Wazuh Server IP> 514
    ```
  - enable & cleanup logging

## chapter 3: technical overview Wazuh

* server filesystem overview
  - logs
  - ossec.conf
  - opensearch data storage
  - rulesets (local_*.xml, custom rulessets, Github rulesets, logtester)
  - binary programs (cleanup and group agents, test logs)
* [Wazuh rulesets](https://documentation.wazuh.com/current/user-manual/ruleset/custom.html)
  - rules and decoders
* index management:
  - indexes overview
  - cleanup alerts after X time

 ## chapter 4: Shuffle workflow automation

 * Wazuh integrations
 * run shuffle and [connect to Wazuh](https://documentation.wazuh.com/current/user-manual/manager/manual-integration.html#shuffle)
 * check integrations.log
