# ansible-role-resize-lvm

This simple ansible role resizes an existing logical volume to match its phsical volume size.

## Usage

```yaml
- hosts: all
  become: true

  roles:
    - role: ansible-role-resize-lvm
      vars:
        vg_name: "ubuntu-vg"
        lv_name: "ubuntu-lv"
        size: "100%PVS"
```
