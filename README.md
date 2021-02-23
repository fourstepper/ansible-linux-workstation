# ansible-linux-workstation

ansible meta-playbook for bootstrapping and managing workstation machines

Check out the various roles used by this playbook [here](https://sr.ht/~fourstepper/ansible-linux-workstation/sources)

## Usage

`ansible-playbook -i inventory --diff -K playbook.yml --vault-password-file=<your_password_file>`

## Vars

See `vars/*` for inspiration and a template.

## CI Tested
**Debian** (testing)

[![builds.sr.ht status](https://builds.sr.ht/~fourstepper/ansible-linux-workstation/commits/debian.yml.svg)](https://builds.sr.ht/~fourstepper/ansible-linux-workstation/commits/debian.yml?)

**Ubuntu** (latest stable)

[![builds.sr.ht status](https://builds.sr.ht/~fourstepper/ansible-linux-workstation/commits/ubuntu.yml.svg)](https://builds.sr.ht/~fourstepper/ansible-linux-workstation/commits/ubuntu.yml?)

**Fedora** (latest release)

[![builds.sr.ht status](https://builds.sr.ht/~fourstepper/ansible-linux-workstation/commits/fedora.yml.svg)](https://builds.sr.ht/~fourstepper/ansible-linux-workstation/commits/fedora.yml?)

**Alpine** (edge, with community repositories enabled)

[![builds.sr.ht status](https://builds.sr.ht/~fourstepper/ansible-linux-workstation/commits/alpine.yml.svg)](https://builds.sr.ht/~fourstepper/ansible-linux-workstation/commits/alpine.yml?)


### Questions

If you have any questions, send an e-mail to the [discuss mailing list](https://lists.sr.ht/~fourstepper/ansible-linux-workstation-discuss)
