---
title: "Home Page"
weight: 20
---

Welcome to the Learn SaltStack Home Page! This site is designed as a living technical reference focussed on SaltStack Config.

The Getting Started section will provide some basic tutorials and links that will help you get started learning SaltStack Config.

<h4>What is SaltStack Config?</h4>

SaltStack Config is a modern configuration management and orchestration tool designed to help customers manage their IT infrastructure. It sits on top of Salt Open and provides a UI into your Salt Infrastructure to help manage jobs and other activities. 

Some key features of SaltStack are:

- <b>Modern Config Management Platform</b> - simple python/YAML system for enforcing configuration across applications and infrastructure.
- <b>Self-Healing</b> - uses event-driven automation to detect and auto-remediate drift.
- <b>Flexible Control</b> - agent and agentless options for managing on-prem, public cloud and network devices.
- <b>Power Toolkit</b> - <a href="https://docs.saltproject.io/en/latest/topics/execution/index.html#:~:text=Salt%20execution%20modules%20are%20called,transferring%20files%2C%20and%20so%20on.&text=Contains%3A%20a%20list%20of%20core%20modules%20that%20ship%20with%20Salt.">remote execution</a> & <a href="https://docs.saltproject.io/en/latest/topics/orchestrate/index.html">orchestration</a> help perform complex tasks like OS Updates, day 2 actions and much more.

<img src="/images/saltconfigarch.png" alt="Architecture">

SaltStack Config is an entitled service for vRealize Automation customers and can be purchased standaone via the vRealize Automation Standard Plus offering. 

<h4>Installing SaltStack Config</h4>

SaltStack Config can be installed via vRealize LifeCycle Configuration Manager and deployed as an appliance. The appliance can either be standalone or vRealize Automation integrated. There is a third installation option still available and that is to install via a .tar file on a standalone Centos 7 or RHEL 7 operating system.

The various methods of installation and the use cases for each one are described <a href="https://docs.vmware.com/en/VMware-vRealize-Automation-SaltStack-Config/8.4/install-configure-saltstack-config/GUID-DBE6D84B-0D4B-4747-8291-B0D80851CE62.html">here</a>.

<h4>Getting Started with SaltStack Config</h4>

Once installed you can start using SaltStack config to push jobs to minions that are associated with various Salt Masters. You can use the build in File Server which is located in Config-->File Server section to create state files or you can create jobs to run state files located in git or locally on the masters in the file roots location (default file roots location is /srv/salt).



