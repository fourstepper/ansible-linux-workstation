# ansible-fedora-workstation

ansible meta-playbook for bootstrapping and managing workstation machines

## Usage

`ansible-playbook -i inventory --diff -K playbook.yml -e personal_fedora=true --vault-password-file=<your_password_file>`

Options for -e are:
- personal_fedora=true
- work_fedora=true
- personal_ubuntu=true
- work_ubuntu=true

- **The options are always "(personal or work)_(name of distro)" as can be seen above**

... and so on.

This is done in such a way so you can have two configurations for the same distribution for different purposes (personal and work), where the_targeted_pc is the configuration file you have made for yourself (template available at machine_configurations/000-template.yml, with some more examples in the same folder)

## CI Tested
**Debian** (testing)

[![builds.sr.ht status](https://builds.sr.ht/~fourstepper/ansible-linux-workstation/commits/debian.yml.svg)](https://builds.sr.ht/~fourstepper/ansible-linux-workstation/commits/debian.yml?)

**Ubuntu** (latest stable)

[![builds.sr.ht status](https://builds.sr.ht/~fourstepper/ansible-linux-workstation/commits/ubuntu.yml.svg)](https://builds.sr.ht/~fourstepper/ansible-linux-workstation/commits/ubuntu.yml?)

**Fedora** (latest + the previous release)

[![builds.sr.ht status](https://builds.sr.ht/~fourstepper/ansible-linux-workstation/commits/fedora.yml.svg)](https://builds.sr.ht/~fourstepper/ansible-linux-workstation/commits/fedora.yml?)

**Alpine** (edge + latest stable)

[![builds.sr.ht status](https://builds.sr.ht/~fourstepper/ansible-linux-workstation/commits/alpine.yml.svg)](https://builds.sr.ht/~fourstepper/ansible-linux-workstation/commits/alpine.yml?)


## Not tested in CI, but should work without a problem
- PopOS 20.04
- PopOS 20.10
- Ubuntu 20.10

### Support

If you have any questions, send an e-mail to the [discuss mailing list](https://lists.sr.ht/~fourstepper/ansible-linux-workstation-discuss)
