---
title: "Accepted"
weight: 5
---

Welcome to the Accepted Keys Page

{{< img src="mainacceptedkeys.png" alt="Keys View" >}}

<h1 style="color:black;font-size:20px;">Accepting a new minion key</h1>

Before you can accept a new minion key, you must first install the minion service on the new machine, and configure it to communicate with the Salt controller. See Prerequisites to accepting keys for more information.

When a user logs in, the SaltStack Config user interface polls the server every 10 seconds for pending minion and Salt controller keys. If a pending key is found, the Minions Key workspace displays the key as pending and alerts the user. These alerts are global, which means you are alerted as you are accessing any workspace in SaltStack Config, not just the Minions Key workspace.

Once a pending key is found, the user interface stops polling for that key type for the duration of the user’s session.

You can also accept keys from the CLI on the Salt Master using the <a href="https://docs.saltproject.io/en/latest/ref/cli/salt-key.html">salt-key</a> command. 

<code>salt-key -a minion1</code> or to accept all keys <code>salt-key -A</code>

Reference: https://docs.saltproject.io/en/latest/ref/cli/salt-key.html

Also keep in mind that keys can also be accepted automatically via a reactor setting or in the master configuration file.



