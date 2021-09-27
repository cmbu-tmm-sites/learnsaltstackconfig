---
title: "Master Keys"
weight: 20
---

Welcome to the Master Keys!

<img src="/Administration/Master_Keys/mainmasterkeypage.png" width="1000" height="700">

The Master Keys section is where keys from the local master or external master systems can be accepted. It is likely that you will deploy many master systems and will want to manage them via SaltStack Config. In order to register the external master systems with SaltStack Config you need to install the <a href="https://docs.vmware.com/en/VMware-vRealize-Automation-SaltStack-Config/8.5/install-configure-saltstack-config/GUID-E5ECC4A0-ABEF-475D-8BF9-53429C0CB6DB.html?hWord=N4IghgNiBcIMIHsB2AzAlgcwK4CcCmABAC4AWhAsmAM5F44EAKEWGaSIAvkA"><i>eAPI plugin</a></i> on the master and then configure the master to point to the SaltStack Config instance. Once you do that then the master will show up as a "Pending" master, once the key is accepted then you can start to manage the minions on that external master as well.

