# Cliente-LDAP
Joining Ubuntu Server to the Windows domain and configuring the LDAP client with SSSD-AD to authenticate AD users.

# Project: Ubuntu Server Integration with Windows Server 2019 Domain
This project aims to integrate an Ubuntu server into a domain managed by Windows Server 2019, enabling centralized authentication via Active Directory and access control through AD groups.

# Project Requirements and Steps
1. Joining the Ubuntu Server to the Domain
Connects the Ubuntu server to the Windows Server 2019 domain, allowing Active Directory users to authenticate on the Linux system.

2. Installing Required Packages on the Linux Server
Installs necessary packages for AD integration, such as sssd, realmd, krb5-user, ldap-utils, and others.

3. Configuring the LDAPS Client with SSSD
Sets up SSSD to use LDAPS (LDAP over SSL), ensuring secure communication with the domain controller.

4. LDAP Configuration
Adjusts configuration files to allow the Linux server to query and authenticate users via LDAP.

5. Adjusting PAM Settings
Modifies PAM (Pluggable Authentication Modules) rules to enable AD user authentication and session control.

6. NSSwitch Configuration
Updates the /etc/nsswitch.conf file to include SSSD for user and group resolution.

7. SSH Configuration Adjustments
Configures the SSH service to allow login from AD users, with appropriate security and access restrictions.

8. AD Group Configuration for Access Management
Creates and defines Active Directory groups that are granted access to the Ubuntu server, simplifying access management.
