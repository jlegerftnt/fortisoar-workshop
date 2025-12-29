---
title: Setup FSR SMTP Connector
linkTitle: Setup SMTP Connector
weight: 30
---

![user_complete_icon](check_box.svg)
We want to setup an SMTP configuration for FortiSOAR communications if not already setup. If this is already setup or you are in an environment with different mail server options then you can just use this as a review to your communication configuration.

---

- Go to **Automation** > **Connectors**. ![Connectors navigation](connectors.png)
- In the Manage Tab search for **SMTP**.
  ![Manage tab](manage_tab.png)

- Open the SMTP connector by clicking anywhere within the highlighted red box.

![Edit SMTP click region](edit_smtp.png?height=400px)

{{% notice tip %}}
This is how you open all connectors, solution packs, and widgets in the Content Hub
{{% /notice %}}

- The default SMTP configuration uses localhost postfix service. We want to configure the connector to match the below settings instead of the default

|                                |                                                 |
| :----------------------------: | :---------------------------------------------: |
|      Configuration Name:       |               `csadmin@fortimail`               |
| Mark as Default Configuration: | _Checked_ ![Check box](checked.png?height=35px) |
|             Host:              |                  `10.100.88.4`                  |
|             Port:              |                       25                        |
|         Default From:          |            `csadmin@financial.local`            |
|           Username:            |                    `csadmin`                    |
|           Password:            |                `$3curityFabric`                 |
|            Use TLS:            |                   _Unchecked_                   |
|            Timeout:            |                       10                        |

![SMTP connector configuration](smtpconn.png)

- If you created a new configuration you should see successful status messages when you save.
  ![Success popup](success.png)
