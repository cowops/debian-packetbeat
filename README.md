Debian-Packetbeat
=================

Packetbeat is an Open Source Application Monitoring and Packet Tracing (Packet Sniffer) system. It works by sniffing the traffic and analyzing network protocols like HTTP, MySQL and REDIS.

Requirements
------------

This role requires a debian compliant system such as ubuntu.

Role Variables
--------------

packetbeat:
    version: "0.3.3"
    url: https://github.com/packetbeat/packetbeat/releases/download/v0.3.3/packetbeat_0.3.3-1_amd64.deb

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: cowops.debian-packetbeat, packetbeat.version: "0.3.3", packetbeat.url: https://github.com/packetbeat/packetbeat/releases/download/v0.3.3/packetbeat_0.3.3-1_amd64.deb }

Tasks
-----

  - Install [packetbeat](http://packetbeat.com/) agent

License
-------

BSD
