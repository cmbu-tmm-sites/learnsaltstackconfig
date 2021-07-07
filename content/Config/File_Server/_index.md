---
title: "File Server"
weight: 204
---

Welcome to the State Files Page

<img src="fileservermain.png" alt="FileServer">

The File Server section is where you can create state files to manage your infrastructure. You can post .sls files, scripts, configuration files and files that you may want to distribute to minions. You can also create them in a variety of scripting languages such as YAML, python, json etc. These files can be accessed via jobs or ad-hoc commands from within SaltStack Config. 

The File Server consists of <a href="https://docs.saltproject.io/en/latest/topics/tutorials/starting_states.html">state files</a> that declare the configuration of your infrastructure. To learn more about State Files click on this link.

When you create state files within this secion they are stored in the SaltStack Config postgres database. The file server also provides a tree like structure to place files and then they can be called by other state files. For instance if you have a state file pushed a configuration file down to a minion the state could look something like this:
<br>
</br>
<img src="/Config/File_Server/samplescriptstate.png">

The source starts with salt:// because that points to the <i>base</i> file roots location.

There are some state file examples and tips here as well <a href="https://blogs.vmware.com/management/2021/06/getting-started-with-saltstack-config-part-1-creating-state-files.html">Getting Started with SaltStack Config: State Files Blog</a>

