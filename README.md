Role Name
=========

A Bind9 role for Designate service

Requirements
------------

None

Role Variables
--------------

Only Openstack controler IP:

* osp_ctl_ip: 192.168.1.9



Example Playbook
----------------


    - name: Setup Bind Service
      hosts: bind
      become: true
      remote_user: ayaseen
      gather_facts: yes
      roles:
        - bind_dns


