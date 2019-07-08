# ansible-rclone
Ansible role to deploy rclone and rclone-based mountpoints

## Pre-requisites

## Variables

## Examples

Install the binary:

    - hosts: servers
      roles:
         - { role: ansible-rclone }

Install the binary and create mountpoints:

    - hosts: servers
      roles:
         - { role: ansible-rclone }
      vars:
         rclone_mounts:
           - remote_src: cloud:data
             dest_path: /srv/data
             os_auth_url: https://cloud.local:5000/v3
             os_tenant_id: a8024d5f228f476cbc654eafc281e0e8
             os_username: jhon
             os_password: doe
