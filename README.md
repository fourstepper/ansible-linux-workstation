# ansible-fedora-workstation

This playbook bootstraps and manages user-critical apps and applications
on a personal workstation

## Usage

`ansible-playbook -i inventory --diff -K playbook.yml -e personal_fedora=true --vault-password-file=<your_password_file>`

Options for -e are:
- personal_fedora=true
- work_fedora=true
- personal_ubuntu=true
- work_ubuntu=true

Where <the_targeted_pc> is the configuration file you have made for yourself (template available at machine_configurations/000-template.yml

Please also review the options in the vars/ folder.

If you are using my roles from the [ansible-workstation group](https://gitlab.com/ansible-opletal/ansible-workstation), you can include your app config files under config_files/<directory_of_app>

## CI Tested
- **Debian** (testing) [![builds.sr.ht status](https://builds.sr.ht/~fourstepper/ansible-linux-workstation/commits/debian.yml.svg)](https://builds.sr.ht/~fourstepper/ansible-linux-workstation/commits/debian.yml?)
- **Ubuntu** (latest stable) [![builds.sr.ht status](https://builds.sr.ht/~fourstepper/ansible-linux-workstation/commits/ubuntu.yml.svg)](https://builds.sr.ht/~fourstepper/ansible-linux-workstation/commits/ubuntu.yml?)
- **Fedora** (latest + the previous release) [![builds.sr.ht status](https://builds.sr.ht/~fourstepper/ansible-linux-workstation/commits/fedora.yml.svg)](https://builds.sr.ht/~fourstepper/ansible-linux-workstation/commits/fedora.yml?)
- **Alpine** (edge + latest stable) [![builds.sr.ht status](https://builds.sr.ht/~fourstepper/ansible-linux-workstation/commits/alpine.yml.svg)](https://builds.sr.ht/~fourstepper/ansible-linux-workstation/commits/alpine.yml?)

## Not tested in CI, but should work without a problem
- PopOS 20.04
- PopOS 20.10
- Ubuntu 20.10
