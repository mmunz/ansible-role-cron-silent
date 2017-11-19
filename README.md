c1.cron-silent
==============

Ansible role to remove unneeded cron log messages.

Currently it removes only one message that is shown before and after each cron run:

- "pam_unix(cron:session): session closed for user root"

Role Variables
--------------

- cron_silent_pam_enabled: yes

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - role: c1.cron-silent
           cron_silent_pam_enabled: yes

License
-------

BSD