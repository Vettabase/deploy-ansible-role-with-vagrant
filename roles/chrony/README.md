# Chrony

This role installs and configures the Chrony time server (for time sincronization).

## Requirements


Ansible version 2.12.6.

## Role Variables


A description of the settable variables for this role (defaults/main.yml).

| Variable                | Required | Default | Choices                   | Comments                                 |
|-------------------------|----------|---------|---------------------------|------------------------------------------|
| ntp_servers             | no      | yes      | list                      | The NTP list of servers                  |
| chrony_package          | no      | yes      | eggs, spam                | The name of Chrony package               |
| chrony_service          | no      | yes      | eggs, spam                | The name of NTP service                  |
| chrony_dir              | no      | yes      | eggs, spam                | The Chrony directory                     |
| chrony_filename         | no      | yes      | eggs, spam                | The name of Chrony config filename       |

## Dependencies

None.

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      become: true
      roles:
         - chorny

## Copyright and Contacts

This repository is distributed under the terms of the GNU GPL, version 3. Copyright: Vettabase Ltd.

To contact us

* info@vettabase.com
* https://vettabase.com

Maintainer: [Aldo Junior](https://github.com/aldoribeirojr)