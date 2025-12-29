---
title: LOOK AT THE PLAYBOOK WE ARE RUNNING TO HANDLE THE IOC HUNT
linkTitle: Handle the IOC Hunt
weight: 20
---

![search_icon](mag_glass.svg)
Inside the **Hunt Record, Demo Hunt – Sunburst Attack**, look to the upper right corner and find the playbook logs icon. ![Playbook Icon](logs.png?classes=inline)
This will open the playbook history for this record. Find the playbook named **Hunt Sunburst IOCs** and open it.

---

1. Look at the **Configuration** step. The **OUTPUT** set the variable called **sunburstIocUrls** to the URL we will use to [download the CSV file](https://raw.githubusercontent.com/sophos-cybersecurity/solarwinds-threathunt/master/iocs.csv). ![Hunt Sunburst Playbook Execution](editsunburst.png)

1. The next step, **Download IOCs CSV File**, has an input configuration to loop on the variable **sunburst_ioc_urls**. ![Download IOC step output](downloadiocs.png)

1. Click the **Edit Playbook** button on the upper right hand corner of the playbook log. Double-click on the **Download IOCs CSV File** step and find the loop configuration.

   |                                           |                                |
   | :---------------------------------------: | :----------------------------: |
   | ![Edit Playbook Button](editplaybook.png) | ![For Loop settings](loop.png) |

1. Close the previous step and double-click on the **Configuration** step and find the configuration settings. ![Variable Configuration](config.png)
