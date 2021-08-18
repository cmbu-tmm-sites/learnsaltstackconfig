---
title: "Minion Keys"
weight: 200
---

<h1 style="color:black;font-size:20px;">Overview</h1>

The Minion Keys workspace is used to manage minion keys. A minion key allows encrypted communication between a Salt Master and Salt minion. The workspace provides an overview of all minions filtered by their respective key states. On initial connection, a Salt minion sends its public key to the Salt Master, which the Salt Master can accept, reject, or deny.

<h1 style="color:black;font-size:20px;">Accessing the Minion Keys Workspace</h1>
To use the Minion Keys workspace, click Minion Keys in the side menu. Minion Keys expands to show the four different key states:

- [Accepted](/Minion_Keys/Accepted)
- [Pending](/Minion_Keys/Pending/)
- [Rejected](/Minion_Keys/Rejected)
- [Denied](/Minion_Keys/Denied)

Select the state for the keys that you are interested in viewing or managing. 

<h1 style="color:black;font-size:20px;">Salt Keys</h1>

For security salt uses RSA and AES keys for minion registration and communication between minion and master. The RSA keys are for authentication and the AES keys provide encrypted communication. The master also sends a rotating AES key that is used to encrypt and decrypt messages sent by the salt master. 

{{< img src="saltkeydiagram.png" width="400" height="500">}}






References:

https://saltstack.gitlab.io/open/docs/salt-user-guide/topics/installation.html#