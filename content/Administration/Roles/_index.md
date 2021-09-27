---
title: "Roles"
weight: 15
---

Welcome to the Roles page!

<img src ="/Administration/Roles/mainrolespage.png" width="600" height="900">

Roles are used to assign permissions to users and groups that will access SaltStack Config UI. SaltStack Config ships with a number of built-in roles and allows you to create custom roles as well. There are three default roles:<br>

<b>User</b> - default role assigned to all users. This role allows for just the most basic permissions like Read Access, view and run jobs and view job history.<br>
<b>Administrator</b> - this role has more advanced permission but primarly focused on system administration. Administrators can view user settings and pillar data, they can also perform operations on resources like jobs and targets. Also they can manage keys.<br>
<b>Superuser</b> - superusers can perform all tasks in the SaltStack Config system. <i>root</i> is also a superuser.<br>

Roles can be granted permission from the various tabs such as Tasks or Advanced. Let's look at the main tabs where permissions can be set.<br>

<h3>Tasks</h3><br>

Tasks allow roles to do things like "Create and delete New Targets" or "Modify Pillar Data".<br>
<br>
<br>
<img src = "/Administration/Roles/tasks.png" width="600" height="900">

