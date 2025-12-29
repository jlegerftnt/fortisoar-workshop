---
title: Incident Response
linkTitle: Incident Response
weight: 5
---

![search_icon](mag_glass.svg)
In this section we’ll explore the Incident Response modules of the system. Click around and checkout the record types inside this record group. Feel free to click: ![Add button](add.png?classes=inline) to see what fields are used for records of the different modules. You can create records and delete records to just get a feel for the system if you like.

---

The Incident Response Group is where we will find records that are often used in SOC operations. We have provided a breakdown of what each module's purpose is.

![Incident Response dropdown](incresp1.png?height=300px)

|  Module Name   |                                                                                           Description                                                                                            |
| :------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|     Alerts     |                Actionable items commonly used for ingestion from other systems. Often contains information that can become indicators that are used to correlate common problems.                |
|   Incidents    |                                                                     Incidents are confirmed impacts from one or more alerts.                                                                     |
|     Tasks      |                                        Tasks are simply a place to store actionable items for individuals or bots and can be related to any other record.                                        |
|   Indicators   | Indicators, sometimes related to confirmed compromise IOCs, are often extracted from alerts. These can often be created from Alerts or Hunts and then used to correlate commonly known problems. |
|   Campaigns    |                                                       Often a collection of incidents that have been isolated back to the same Bad Actor.                                                        |
|     Hunts      |                                    A record to kick off an initiative to hunt for problems and then correlate to existing or not found alerts and indicators.                                    |
|   War Rooms    |                                                      A place to kick off an official communication channel to stakeholders in an incident.                                                       |
| Communications |                                                           Module to track external communications with third party chats, emails, etc.                                                           |
