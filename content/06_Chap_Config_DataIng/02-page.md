---
title: CONFIRM FORTIANALYZER HAS EVENTS
linkTitle: Confirm Events
weight: 10
---

![search_icon](mag_glass.svg)
We want to make sure that the FAZ has some events. These are events that we want to be handled via FortiSOAR to turn into to
You should see new events last updated “**A few seconds ago**”.

---

1. Access the FortiAnalyzer by clicking on the **Enterprise FortiAnalyzer** **HTTPS** button from your demo instance or by browsing to `https://<your instance>.fortidemo.fortinet.com:14003/` ![HTTPS page](enterprise_faz.png).
2. Sign in with fortinet/`$3curityFabric`
3. Go to **Incidents & Events > Events Monitor**
4. Confirm you see botnet events created with Medium or High Severity

{{% notice note %}}
Events may take a few minutes to appear.
{{% /notice %}}

![Faz event grid display](fsoc.png)
