---
title: IMPORT POLICIES FROM THE FORTIGATE CONFIG
linkTitle: Import Policies
weight: 20
---

![search_icon](mag_glass.svg)

We now have a new module to store policy information and the ability to connect with the FortiGate API. The next step is to extract polices as records from the FortiGate configuration to then be audited during a SOC Policy Review.

---

![user_complete_icon](check_box.svg)

1. Inside **Resources>Policies** click on the **Execute** button and run the playbook called **Import FortiGate Policies**. ![](fgtpol.png?height=300px)

2. When complete you should have new Policy records added to your Policies module that match your FortiGate Config. ![](fwpol.png?height=400px)
