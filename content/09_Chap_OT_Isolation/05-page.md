---
title: Isolate Device
linkTitle: Isolate Device
weight: 50
---

![Check Box](check_box.svg)
We will now use the other imported playbooks in this Chapter by running them against an alert

---

## Navigate and Fix Columns

1. Navigate to **Resources > Assets**
   ![Assets](assets_nav.png)

1. Click the Hamburger icon on the top row of the grid ![Hamburger Icon](hamburger_icon.png?classes=inline) , look for the field **Asset State** and click it.
   ![Assets](asset_state_column.png)

{{% notice tip %}}
You may need to zoom out from your browser to see the column. You can click and hold the column name and drag it to move the column to the left or right of other columns
{{% /notice %}}

1. Once done your columns should look something like the image below
   ![Assets Columns](asset_columns.png)

## Isolate a Device

1. Select the checkbox of any Asset record with **Asset Type** of **OT**
1. Click the Execute button and Click **Isolate Device**
   ![Isolate Device](isolate_asset.png)

1. Click the clipboard icon at the top right
1. Click the text **Are you sure you want to isolate**
   ![Manual Input](manual_input.png)
1. Click yes to confirm isolating the playbook
   ![Isolate device](isolate_confirm.png)

{{% notice note %}}
What happens when you try execute the **Isolate Device** playbook on a **Asset** that has the type **IT** ?
{{% /notice %}}

## Check the Results

1. Access the FortiGate by clicking on the **Enterprise_Core** **HTTPS** button from your demo instance or by browsing to `https://<your instance>.fortidemo.fortinet.com:14002/` ![HTTPS page](enterprise_core.png)

1. Navigate to **Policy & Objects > Firewall Policy**
1. Hover over the **OT Isolated** group to confirm you see the IP of the asset you isolated previously
   ![isolated_group](isolated_group.png)
