---
title: Find the Malicious URL Indicator and Block it
linkTitle: Block Malicious Indicator
weight: 25
---

![user_complete_icon](check_box.svg)
In this **Alert** we can see that we obtained an email and extracted various “indicators” and created a separate **Indicator** record for each. Now that this has been done we can see the linked indicators towards the bottom of the Alert record.

---

1. Inside the **Alert**, navigate to the bottom of the record and look for the **Indicators tab**. ![Indicator Relationships](alert81.png?height=300px)

2. Find the **URL Type Indicator** named `http://demo.gumblar.cn/` and drill into this record. ![IOC detail view](gumblar.png)
   {{% notice note %}}Notice that when inside an indicator record from the alert record we see “Alert -> Indicator” as our path at the top. This can be used to help navigate you back to the original alert which would be “less clicks” than closing out the window and finding the alert again when you are done with the indicator.{{% /notice %}}

3. Inside this opened **Indicator** record look for the Execute button at the bottom of the record ![Execute Button](exec.png) and Execute the “**Block URL**” playbook. ![Execute button Options](blockurl.png?height=300px)

{{% notice note %}}If you do not have a **Block URL** option make sure you selected a “**URL Type**” indicator. Execute buttons can be selectively shown based on type of record.{{% /notice %}}

1. Follow the prompts to **Block** and then indicate the **Block Completed** and the status of this indicator should go to “Blocked”. ![Block display 1](blockurl1.png?height=200px) ![Block Display 2](blockcompleted.png?height=200px)

{{% notice note %}}In a production environment the “Block Complete” step should be configured to actually use a connector, like a FortiGate, for efficiency {{% /notice %}}
