---
title: "Authentication"
weight: 10
---

Welcome to the Authentication Page

<img src="/Administration/Authentication/authenticationmain.png" width="600" height="700">

<h1 style="color:black;font-size:20px;">Overview</h1>
<br>
The Authentication workspace allows administrators to configure user identity and access management for SaltStack Config. Using this workspace you can configure various authentication integrations:

 - Single Sign-On authentication (SSO) for an Identity Provider (IdP) that uses the SAML or OAuth protocols.
 - Access management for directory services that use the LDAP protocol, such as Active Directory Domain Services.

<h1 style="color:black;font-size:20px;">Configuring LDAP Connection</h1>
<br>
<table style="width:100%">
  <tr>
    <th>Field</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>Name</td>
    <td>Name of LDAP Connection</td>
  </tr>
  <tr>
    <td>Host</td>
    <td>LDAP Host Server Address</td>
  </tr>
  <tr>
    <td>Port</td>
    <td>Port where LDAP server is configured. Default is 389.</td>
  </tr>
  <tr>
    <td>Background Sync</td>
    <td>SaltStack Config validates all users and group against this authnetication in set interval</td>
  </tr>
  <tr>
    <td>Auth Base DN</td>
    <td>Base LDAP Name ex.: DC=corp,DC=local,DC=com</td>
  </tr>
  <tr>
    <td>Admin Bind DN</td>
    <td>Administrator DN ex.: cn=Admin,cn=Users,dc=corp,dc=local</td>
  </tr>
  <tr>
    <td>Auth Bind DN Filter</td>
    <td>Filter applied to select a specific user. ex.: (objectclass=person)
  </tr>
</table>

