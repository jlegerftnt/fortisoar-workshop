---
title: Prepare the FortiGate via a playbook
linkTitle: Run Playbook
weight: 40
---

![Check Box](check_box.svg)

The new OT collection has a playbook that will configure multiple things on the **Enterprise Core** FortiGate. This work has been done ahead of time to speed up the workshop.

In OT environments there is heavy red tape around blocking new traffic. In short, all OT devices _must_ be able to communicate to other OT devices. If there is malware identified on an OT device, the spread should be _mitigated_ and not blocked outright. This is what the policy above does. The policy will _only_ allow **isolated** OT assets to communicate to devices in the OT Assets group, and nothing else.

---

## Run the playbook

1. Open the playbook **Step 1. Prep FortiGate**
   ![Prep playbook](new_playbook.png)

1. Observe the steps in the playbook. It is documented with the tasks it will perform
   ![Prep playbook 2](prep_playbook.png)

1. Run the playbook by clicking the start button ![Run playbook](start_playbook.png)
1. Click Trigger Playbook to confirm
   ![Trigger Playbook](trigger_playbook.png)

## Confirm the changes on the FortiGate

1. Access the FortiGate by clicking on the **Enterprise_Core** **HTTPS** button from your demo instance or by browsing to `https://<your instance>.fortidemo.fortinet.com:14002/` ![HTTPS page](enterprise_core.png?height=300px)

1. Navigate to **Policy & Objects > Firewall Policy**
1. Confirm that you see a new policy at the top
   ![New policy](ot_policy.png)

1. Edit the policy **Block OT isolated to non OT**
   ![Policy Details](policy_negate.png)

{{% notice note%}} This policy is a destination address negate policy.
{{% /notice %}}
