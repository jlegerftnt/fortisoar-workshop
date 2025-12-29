---
title: Setup FortiMail
linkTitle: Setup FortiMail
weight: 5
---

![user_complete_icon](check_box.svg)
In this workshop we will use FortiMail as our SMTP server.

- Access the FortiMail admin access by clicking on the "Corporate FortiMail" **HTTPS** button from your demo instance or by browsing to `https://<your instance>.fortidemo.fortinet.com:14001/admin/`
  ![HTTPS page](fortimail_https.png)

- Login with user/pass: fortinet/`$3curityFabric`
  ![Login Screen](fortimail_login.png)

- Locate the **fortisoar-workshop-fortimail-users.csv** file that is in your downloaded `all_files` folder

- Navigate to the **Domain & User > User section** and import the _fortisoar-workshop-fortimail-users.csv_ file by clicking **Import CSV** and uploading the file
  ![FortiMail User Page](fml_setup.png)

{{% notice note %}}
You should now have FortiSOAR users in FortiMail. If you do not, you may need to refresh (F5) the page.
{{% /notice %}}
