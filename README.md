[![Build Status](https://travis-ci.org/CSC-IT-Center-for-Science/ansible-role-nfs_mount.svg)](https://travis-ci.org/CSC-IT-Center-for-Science/ansible-role-nfs_mount)
ansible-role-nfs_mount
=========

Mounts NFS 

Requirements
------------

An NFS server

Role Variables
--------------

all:
<pre>

nfs_mount_point:
  - /data0
  - /data1


nfs_mount: |
  10.2.1.5:/scratch /scratch                nfs4 defaults 0 0
  10.2.1.5:/home    /home                   nfs4 defaults 0 0
  10.2.1.6:/data0   /data0                  nfs4 defaults 0 0
  10.2.1.6:/data1   /data1                  nfs4 defaults 0 0

</pre>

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: ansible-role-nfs_mount }

License
-------

MIT

Author Information
------------------
