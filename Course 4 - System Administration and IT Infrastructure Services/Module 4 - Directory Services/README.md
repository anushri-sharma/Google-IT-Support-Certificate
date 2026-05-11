## Directory Services

In the fourth week of this course, we'll learn about directory services. Specifically, we'll cover how two of the most popular directory services, Active Directory and OpenLDAP, work in action. We'll explore the concept of centralized management and how this can help SysAdmins maintain and support all the different parts of an IT infrastructure. By the end of this module, you will know how to add users, passwords, and use group policies in Active Directory and OpenLDAP.

### Key Concepts

* Understand what services a directory server provides.
* Understand what LDAP and Active Directory are.


------

AAA (authentication, authorization, accounting): The services that the directory services provide
to all the computers within a company or organization

Active directory (AD): The Microso alternative to directory services that oers customization and
added features for the Windows plaorm

Active directory users and computers (ADUC): The client tools that are used for accessing and
administering a directory server

Advanced group policy management (AGPM): A set of add-on tools from Microso that gives some
added provision control abilities in GPMC

Bind operation: The operation which authenticates clients to the directory server

Central management: A central service that provides instructions to all of the dierent parts of my IT
infrastructure

Change management process: The process to notify others in the organization about the changes
that you are about to make

Computer conguration: Contained within a Group Policy Object (GPO)

Conguration management: The creation of rules about how things should work in your organization,
such as printers, congure soware, or mounting network le systems

Default domain control policy: One of the two GPOs that are created when a new Active Directory
domain has been made

Delegation: The administrative tasks that you need to perform a lot as a part of your day to day job
but you don't need to have broad access to make changes in AD

Directory Access Protocol (DAP): A protocol that is included in the X.500 directory standard from
1988

Directory Information Shadowing Protocol (DISP): A protocol that is included in the X.500 directory
standard from 1988

Directory Operational Bindings Management Protocol (DOBMP): A protocol that is included in the
X.500 directory standard from 1988

Directory server: The server that contains a lookup service that provides mapping between network
resources and their network addresses

Directory services: A lookup service contained in a network server that provides mapping between
network resources and their network addresses

Directory System Protocol (DSP): A protocol that is included in the X.500 directory standard from
1988

Distribution group: A group that is only designed to group accounts and contacts for email
communication

DNS records: A DNS request for the SRV records matching the domain that it's been bound to

Domain admin: The administrators of the Active Directory domain

Domain computers: All the computers joined to the domain except domain controllers

Domain controllers (DC): The service that hosts copies of the Active Directory database

Domain local: The tool used used to assign permission to a resource

Domain users: A group that contains every user account in the domain

Enterprise admin: The administrators of the Active Directory domain that has permission to make
changes to the domain that aect other domains in a multi-domain forest

Enterprise mobility management (EMM): A system that can create and distribute policies and MDMs

Fast logon optimization: The group policy engine that applies policy seings to a local machine may
sacrice the immediate application of some types of policies in order to make logon faster

Flexible single-master operations (FSMO): The single domain controller that has been tasked with
making changes to the AD database that can only be made by one DC at a time

Forest: The hierarchy above a domain that contains multiple domains, allowing accounts to share
resources between domains that are in the same forest

Functional levels: The dierent versions of Active Directory, a functional level that describes the
features that it supports

Global: The tool that is used to group accounts into a role

Group policy management console (GPMC): The tools used for creating and viewing a group policy
object

Group policy objects (GPO): The ways to manage the conguration of Windows machines, referring
to the objects that represent things in your network that you want to be able to reference or manage

Group policy seings reference: A spreadsheet that details the GPO policies and preferences that
are available and where to nd them

Group scope: The way that group denitions are replicated across domains

Import: Moving a backup of the test example policy to the production example policy

Kerberos: A network authentication protocol that uses tickets to allow entities to prove their identity
over potentially insecure channels to provide mutual authentication

LDAP data interchange format: The tool that allows you to authenticate, add, remove users, groups,
computers and so on in a directory service

LDAP Entry: A collection of information that's used to describe something

LDIF les: A text le that lists aributes and values that describe something

Lightweight Directory Access Protocol (LDAP): An open industry-standard protocol for accessing
and maintaining directory services; the most popular open-source alternative to the DAP

Linked: A GPO that all of the computers or users under a domain, site, or OU will have a policy applied


MDM policy: The proles that contains seings for the device

MDM prole: The policies that contains seings for the device

One-way cryptographic hash: The method used by AD to store passwords

OpenLDAP (lightweight directory access protocol): An open source and free directory service

Organizational units (OU): A hierarchical model of objects and containers that can contain objects or
more organizational units

Parent group: Groups that are principal groups and contain other groups

PHPLDAPadmin: A tool to manage OpenLDAP

Policies: Seings that are reapplied every few minutes, and aren’t meant to be changed even by the
local administrators

Precedence: When computers are processing the Group Policy Objects that apply to them, all of
these policies will be applied in a specic order based on a set of precedents rules

Read-write replicas: Domain controllers in the Active Directory network that each have a complete
copy of the AD database and are able to make changes to it

Remote wipe: A factory reset that you can trigger from your central MDM rather than having to do it in
person on the device

Replication: the store directory data is copied and distributed across a number of physically
distributed servers but still appears as one unied data store for querying and administering

Replication failure: A reason that a GPO might fail to apply as expected

Reset: When an SysAdmin restores or resets the password of a user

Restart: A command that will let the machine reboot to complete a domain join

Resultant set of policy (RSOP): The policy that forms when all of the group policies have been
grouped together for a specic machine and apply precedence rules to them

Role-based access control (RBAC): The process of changing a persons group that they are a part of
when they have changed roles within a company to limit or change their access to resources

RSOP report: The process of troubleshooting group policy and comparing what you expect to be
applied to a computer and the resultant set of policy report

Security account manager (SAM): A database in windows that stores user names and password

Security ltering: A tool to make group policies apply more selectively

Security group: One of the two categories that groups in Active Directories can be part of, they can
contain user accounts, computer accounts or other security groups

Security principal: Any entity that can be authenticated by the system, such as a user account, a
computer account, or a thread or process that runs in the security context of a user or computer
account

Service discovery: One of the services that the domain controller provides to the clients

Simple authentication and security layer (SASL): The authentication method that can employ the
help of security protocols like TLS, it requires the client and the directory server to authenticate using
some method

SRV records: A service record used to dene the location of various specic services

Systems administrator (sysadmin): A person who works only in system administration, conguring
servers, monitoring the network, provisioning, or seing up new users in computers and taking
responsibility of systems

Universal: The tool that is used to group global roles in a forest

User conguration: Contained within a Group Policy Object (GPO)

User Groups: The management of resources on a computer and on a network through organizing user
accounts into various groups

Windows management instrumentation (WMI): The container that is used to dene powerful
targeting rules for your GPO

Windows registry: A hierarchical database of seings that Windows, and Windows applications, use
for storing conguration data

WMI lter: A tool to make group policies apply more selectively on the conguration of the computer

Work group computer: A Windows computer that isn't joined to a domain

X.500 directory: The agreed upon directory standard that wa approved in 1988 that includes, DAP,
DSP, DISP, DOP, DAP, and LDAP
