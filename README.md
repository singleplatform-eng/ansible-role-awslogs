
ansible-role-awslogs
=========

Ansible role for installing and configuring the CloudWatch Logs Agent

Role Variables
--------------

- `awslogs_config`: list of log files to monitor

    Example:
    
        awslogs_config:
          - file: /var/log/syslog
            datetime_format: "%b %d %H:%M:%S"
            log_group_name: syslog

Example Playbook
----------------

    - hosts: all
      become: yes
      roles:
          - ansible-role-awslogs

Author Information
------------------

[SinglePlatform Engineering](http://engineering.singleplatform.com/)

License
-------

BSD 3-Clause
