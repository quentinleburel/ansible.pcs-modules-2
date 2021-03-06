pcs-modules-2
=============

Modules for configuring pacemaker cluster on CentOS/RHEL 6/7 systems.

Requirements
------------

RHEL: It is expected that machines will already be registered and subscribed for access to 'High Availability' or 'Resilient storage' channels.

Role Variables
--------------

None. This role is intended to be included as dependency.

Provided Modules
----------------

*pcs_auth* - (de)authorization of nodes in pacemaker cluster

*pcs_resource* - create/update/delete cluster resources in pacemaker cluster including stonith resources

*pcs_constraint_location* - create/delete cluster location constraints in pacemaker cluster

*pcs_constraint_colocation* - create/delete cluster colocation constraints in pacemaker cluster

*pcs_constraint_order* - create/delete cluster order constraints in pacemaker cluster

*pcs_cluster* - create/destroy pacemaker cluster

*pcs_property* - set/unset pacemaker cluster properties

Example Playbook
----------------

Example playbook for including modules in your playbook

    - hosts: servers
      roles:
         - { role: OndrejHome.pcs-modules-2 }

License
-------

GPLv3 or Apache License 2.0, check LICENSE file for more information

Author Information
------------------

WARNING: This was not tested extensively and may brake. Recommended use is for testing only.

To get in touch with author you can use email ondrej-xa2iel8u@famera.cz or create a issue on github when requesting some feature.
