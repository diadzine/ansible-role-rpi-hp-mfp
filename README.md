Ansible Role: RPi HP Multifunction Printer
==========================================

[![Build Status](https://travis-ci.org/diadzine/ansible-role-rpi-hp-mfp.svg?branch=master)](https://travis-ci.org/diadzine/ansible-role-rpi-hp-mfp)

Ansible role to install Cups and hplip on Raspbian-based Raspberry Pi machines.

Requirements
------------

None.

Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

    raspberry_pi_update_packages: yes

Boolean to set if you want to run apt update before installing packages.

    apt_packages:
      - avahi-daemon
      - cups
      - cups-pdf
      - python-cups
      - hplip
      - sane

List of packages that will be installed on the system using apt. Here are the default packages.

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: pi
      roles:
         - { role: diadzine.rpi-hp-mfp }

License
-------

MIT License.

Author Information
------------------

This role was created in 2018 by [Aymeric Bringard](https://github.com/diadzine/).
