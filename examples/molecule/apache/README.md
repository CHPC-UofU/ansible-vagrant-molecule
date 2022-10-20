
Ansible Role: Apache Web Server
=======================================================

Ansible role to configure a basic Apache instance.

## Requirements

None

## Role Variables

Defaults for the variables below may be found in `defaults/main.yml`:

* `apache_enabled`: whether the initial Apache service state is enabled
    * Default value: `yes`
    * Recommended values: `yes`, `no`
* `apache_packages_state`: installation state for the Apache packages
    * Default value: `present`
    * Recommended values: `present`, `latest`
* `apache_state:`: initial Apache service state
    * Default value: `started`
    * Recommended values: `started`, `stopped`

## Dependencies

None

## Example Playbook

See `./molecule/default/converge.yml`.

## License

Unlicense

## Author Information

Maintained by the crew of the Rocinante.
