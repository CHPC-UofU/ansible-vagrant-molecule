
Ansible Role: Apache Web Server
=======================================================

Ansible role to configure a basic Apache instance.

* In this directory use `./test-settings.yml` to control multiple operating system and versions for the virtual machines under test.
* View the default web page at [https://localhost:8440](https://localhost:8440) (if multiple VMS are created concurrently each VM will get its own port, `8440`, `8441`, `8442`, and so on).
* Lint the Ansible Role by referencing the test playbook. For example:
  ```shell
  (python-env) user@machine vagrant $ ansible-lint -p ./test-playbook.yml
  
  Passed with production profile: 0 failure(s), 0 warning(s) on 9 files.
  ```

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

See `./test-playbook.yml`.

## License

Unlicense

## Author Information

Maintained by the crew of the Rocinante.
