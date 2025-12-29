---
title: Onboard a FortiGate
linkTitle: Onboard a FortiGate
weight: 50
---

![search_icon](check_box.svg)
In this section we’ll onboard a FortiGate manually so that it checks into FortiManager. Onboarding a device to FortiManager can be done automatically using various methods (DHCP option, FortiZTP, FortiDeploy SKU), but we’ll do it manually for this lab.

---

{{% notice warning %}}
Do not Authorize Branch1. We will do that later.
{{% /notice %}}

## Onboard a FortiGate

1. Login to Branch1 using admin/`$3curityFabric`
2. Navigate to **Security Fabric > Fabric Connectors**.
3. Click **Central Management**
   - Click **Enabled**
   - Type `10.100.88.10` in the **IP Address** field.
   - Click OK

![Authorize FMG](authorize_fmg.png)

## Confirm FortiGate is unauthorized in FortiManager

1. Login to FortiManager using admin/``$3curityFabric```
2. Navigate to **Device Manager > Unauthorized Devices**
3. Confirm that the Branch1 FortiGate is listed

{{% notice warning %}}
Do not Authorize Branch1. We will do that later.
{{% /notice %}}

![Unauthorized branch1](unauthed_devices.png)

## Create Policy Package

1. Navigate to **Policy & Objects > Policy Package**
2. Select **Policy Package** and click **New**
   ![create_policy_package](create_policy_package.png)
3. Type in `Golden_Branch` for the **Name** and click **OK** at the bottom of the page.

## Create Policy

1. Select **Policy Packages > Golden_Branch > Firewall Policy**
   ![golden_branch](golden_branch.png)
2. Click **Create New > Create New** to create a new policy
   ![create_new_policy](create_new_policy.png)
3. Set the following fields on the _Create New Firewall Policy_ page (leave the rest as default):
   - **Name**: `Allow port2 to Internet`
   - **Incoming Interface**: `port2`
   - **Outgoing Interface**: `port1`
   - **Source**: `RFC1918-10`
   - **Destination**: `all`
   - **Service**: `HTTPS`
   - **Action**: `Accept`
   - **NAT**: `Enable`
   - **Change Note**: `Policy Creation`
4. Click **OK** at the bottom of the page.

You now have your first policy!
![new_policy](new_policy.png)
