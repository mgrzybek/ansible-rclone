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
           - name:
             remote_src:
             dest_path:
