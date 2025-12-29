---
title: TRIGGER SOME LOGS FROM THE FGT
linkTitle: Trigger Logs
weight: 5
---

![user_complete_icon](check_box.svg)

1. Access the FortiGate by clicking on the **Enterprise_Core** **HTTPS** button from your demo instance or by browsing to `https://<your instance>.fortidemo.fortinet.com:14002/` ![HTTPS page](enterprise_core.png)
2. Sign in with fortinet/`$3curityFabric`

3. Access the integrated ssh via the button at the top right.
   ![Fortigate ssh button](fortigate_ssh.png)

4. Run the command “**diagnose log test**” in the CLI console. This will kick off some test events from the FG and will show up. Run the command about 3x in a row to generate more logs.

![cli command and output](cli.png)
