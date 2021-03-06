.. include:: <xhtml1-lat1.txt>
`Home <index.html>`__ |raquo| Security hardening for openstack-ansible

Security benefits FAQ
=====================

The openstack-ansible-security role provides hardened security configurations
for the host operating system as well as many common system services.

Why should this role be applied to a system?
--------------------------------------------

First and foremost, this role should be applied to production systems in
environments where security is a priority.  If an OpenStack environment is
exposed to the internet or to large internal corporate networks, applying
this role will reduce the risk of compromised OpenStack infrastructure. The
changes made by the role should also reduce the impact of potential
compromises as well.

Some deployers may be subject to industry compliance programs, such as
PCI-DSS, ISO 27001/27002, or NIST 800-53.  Many of these programs require
hardening standards to be applied to critical systems, such as OpenStack
infrastructure components.

What systems are covered by openstack-ansible-security?
-------------------------------------------------------

At this time, the openstack-ansible-security role provides security hardening
for physical servers running Ubuntu 14.04.  The containers that run various
OpenStack services on these physical servers are currently out of scope.

Virtual machines that are created within the OpenStack environment are also
not affected by this role, although this role could be applied within those
VM's if a deployer chooses to do so.
