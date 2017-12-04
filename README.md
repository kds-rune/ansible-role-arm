# Ansible Role: arm

A simple role to install the 'automatic ripping machine' (`https://github.com/ahnooie/automatic-ripping-machine`)

## Requirements

None

## Role Variables

None

# Dependencies

None

# Example Playbook
```yaml
- hosts: army-of-arms
  gather_facts: True
  tasks:

  - include_role:
      name: noruro.arm
    vars:
      arm_mkv_args: '--profile=/opt/arm/default.mmcp.xml'
      arm_mkv_profile: '-sel:all,+sel:(nor|nob|eng),-sel:(havemulti),-sel:mvcvideo,=100:all,-10:favlang,-20:nor,-30:nob'
      arm_hb_args: '--subtitle-lang-list nob,eng --all-subtitles --subtitle scan -F --audio-lang-list nob,eng,und --all-audio'
      arm_plex_extras: 'true'
```
# License

MIT

Author Information

N/A
