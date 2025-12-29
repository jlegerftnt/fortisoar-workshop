---
title: INVESTIGATE THE PLAYBOOKS RELATED TO THIS INDICATOR
linkTitle: Investigate the Playbooks
weight: 30
---

![search_icon](mag_glass.svg)
Inside the same **Indicator** look to the upper right corner and find the playbook logs icon. ![Playbook Execution History Icon](logs.png)

This will open the playbook history for this record. Find the playbooks that have run and open one. This screen may vary as these playbooks come from the **SOAR Framework Solution Pack** and can be changed from the content hub.

Click on any of the steps to see what each step could see for the input and output. Click the **ENV** button to see what the playbook as a whole could "see" during this execution. ![ENV button](env.png)

---

1. Follow the results of the playbook from the playbook log. Look for an example that Enriches the Indicator, such as the one called “**URL / Domain > Fortinet Web Filter Lookup > Enrichment**” from this screenshot. ![Playbook Log Detail](enrich.png?height=400px)

1. Click on the steps from the log and hit the ENV to see what the playbook can see. ![ENV results](playbook1.png?height=400px)

1. Click on a couple of the steps and look at the **Input** and **Output** Tabs to see what the step could see. Close the **Execute Playbook Logs** window when done looking around. ![Step output](playbooklogs.png?height=300px)
