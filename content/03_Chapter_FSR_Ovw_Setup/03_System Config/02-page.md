---
title: Confirm & Edit the System Notification Channel
linkTitle: System Notification Channel
weight: 35
---

![user_complete_icon](check_box.svg)
We want the system to use FortiMail as the SMTP host for email notifications. We will make this change inside the Notification Channel if needed. We will test our notification channel with a system user in a future step.

---

1. Navigate to System Settings (Gear Icon at the top right). ![System Settings Icon](topright.png)

2. Go to **System > Notifications > Notification Channels** and _double click_ the text **Email Notification** to open the record ![Email Notification](email_notification.png)

3. Click the continue button.![Continue button](continue.png?height=40px&classes=left)

{{% notice note %}}
If not set to SMTP then change the “Choose suitable configured connector” to SMTP. If the SMTP config is set to **localhost-postfix** modify the SMTP Configuration to use **csadmin@fortimail**.
{{% /notice %}}

1. Click ![Continue Button](continue.png?height=40px&classes=left,inline) at the bottom right until you can click ![Save Button](save.png?height=40px&classes=left,inline)

![Update Channel](update.png)

---

![search_icon](mag_glass.svg)

### Bonus Points :money_with_wings:

- Navigate to **System > Notifications > Delivery Rules**
  - Edit a delivery rule. How will the notification activate?
  - What will the notification do when it is activated?
