---
title: "Denied"
weight: 200
---

Welcome to the Denied Page

<h1 style="color:black;font-size:20px;">Overview</h1>

Denied keys were automatically rejected by the Salt Master. This occurs when a minion has a duplicate ID, or when a minion was rebuilt or had new keys generated and the previous key was not deleted from the Salt Controller. If this happens, delete the denied key to trigger a new key regeneration. In this state, connections are not accepted from the minion and jobs are not executed.