---
title: Update Connector Config for VirusTotal
linkTitle: Update Connector for VT
weight: 60
---

![user_complete_icon](check_box.svg)
Earlier in this lab you should have retrieved an API token for your VirusTotal account. You will use this here.

---

- Go to Automation and Connectors. ![Automation Dropdown](connectors.png)

- In the Manage Tab search for “virustotal”

- Edit the connector configuration to have your Virus Total API Key from section [External Requirements - External Accts]({{% relref "/02_chapter_ext_reqts/02-page.md#virustotal" %}}) . You can call the configuration whatever you like – in this lab we called it “mylab”. ![Virustotal Connector Configuration page](vtconn.png?height=500px)

- Paste in your API key to the _API Key_ field

- Click save and you should see an Available Health Check Status.
  ![Success status for virustotal ](vtstatus.png)
