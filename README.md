grub_cmdline_options
====================

This role ensures that grub options are added to the `GRUB_CMDLINE_LINUX_DEFAULT` variable in `/etc/default/grub`.
Please be aware that this role does not manage the removal of options!

As always: Use at your own risk!

Role Variables
--------------

| Name                         | Comment                                              | Default value |
|------------------------------|------------------------------------------------------|---------------|
| grub_cmdline_options_present | A list of options to be present for the linux kernel | `[]`          |

Example Playbook
----------------
```yaml
- name: Configure Grub boot manager
  hosts: clients
  roles:
    - role: oxivanisher.linux_base.grub_cmdline_options
```

License
-------

BSD

Author Information
------------------

This role is part of the [oxivanisher.linux_base](https://galaxy.ansible.com/ui/repo/published/oxivanisher/linux_base/) collection, and the source for that is located on [github](https://github.com/oxivanisher/collection-linux_base).
