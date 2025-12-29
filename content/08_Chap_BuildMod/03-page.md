---
title: CREATE AN API ACCOUNT ON THE FORTIGATE
linkTitle: Create API Acct
weight: 15
---

![user_complete_icon](check_box.svg)
We want to create a new API Admin, called **“fortisoar”** to use the Fortigate API and extract existing policies from the configuration

---

1. Access the FortiGate by clicking on the **Enterprise_Core** **HTTPS** button from your demo instance or by browsing to `https://<your instance>.fortidemo.fortinet.com:14002/` ![HTTPS page](enterprise_core.png)

2. Navigate to **System > Administrators**

3. Create a **New Rest API Admin**, called “**fortisoar**”, in your **Enterprise_Core** FortiGate, using the Administrator profile of **api_full** and hit OK to get your API Key. ![](restadmin.png?height=300px)

4. Save **Your New API Key** to be used in a FortiSOAR connector config. ![](genapi.png)

---

4. Back to FortiSOAR, go to **Automation>Connectors>Manage** and search for “**FortiGate**” and open the “**Fortinet FortiGate Custom**” connector. ![](autoconn.png?height=300px)

5. Make sure the hostname matches “**10.100.88.1**“ and click **Set API Key** to set the Key you obtained for the “fortisoar” API user from the FortiGate.

|                 |                                 |
| :-------------: | :-----------------------------: |
| ![](setkey.png) | ![](fgtcustom.png?height=400px) |

1. After you save you should see a successful status message. ![](confconn.png?height=300px)
