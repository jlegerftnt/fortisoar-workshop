---
title: IMPORT THE SOLUTION MODULE(S) WITH PLAYBOOKS
linkTitle: Import Modules
weight: 5
---

![user_complete_icon](check_box.svg)
Locate the **FortiSOAR-SE_Training2023-PolicyModule.zip** file that is in your downloaded `all_files` folder. This is a solution that we can import into your FortiSOAR instance to handle our policy management use case.

---

1. Navigate to System Settings (Gear Icon at the top right). ![System Settings Icon](topright.png)

2. Scroll on the left pane to the bottom and click Import Wizard. ![Import Wizard Option](impwiz.png?height=400px)

3. Click Import from File. ![Import from File Icon](impfile.png?height=200px)

4. Click into the dashed box to open the file explorer or drag the file **FortiSOAR-SE_Training2023-PolicyModule.zip** into the upload box. ![File Import By selecting file](fileexp.png?height=400px)

5. Click ![Continue Button](continue.png?height=40px&classes=left,inline) at the bottom right until you can click ![Run Import button](runimp.png?classes=left,inline)

6. Click “**I have reviewed the changes – Publish**”. ![Review Publish Popup](revpub.png?height=300px)

7. Wait for the import to finish
   ![Import Status](import_status.png?height=300px)

---

*** Import Playbook ***

The solution module import creates the policy module, but we also need to import the updated playbook that will be used later in this chapter.

1. Navigate to **Automation > Playbooks** from the left-side navigation menu.

2. In the Playbooks search field, search for **00 - Policy Playbooks Collection**. Open the matching collection so you are importing the playbook into the correct collection.
   ![Policy playbook collection](<Policy playbook collection.png?height=300px>)

3. Click the **Import** button in the playbook collection toolbar.
   ![Import Playbooks button](<Import Playbooks.png?height=300px>)

4. In the import window, upload the **Update Fortigate Policy Playbook.json** file from your downloaded files.

5. When prompted for the import behavior, select **Replace Existing Playbooks**. This ensures the existing workshop playbook is overwritten with the updated version instead of creating a duplicate or leaving the older version in place.
   ![Replace existing playbooks option](<Replace playbook.png?height=300px>)
