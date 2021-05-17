# ansible-linux-workstation

[![CI](https://github.com/fourstepper/ansible-linux-workstation/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/fourstepper/ansible-linux-workstation/actions/workflows/ci.yml)

ansible meta-playbook for bootstrapping and managing workstation machines

Check out the various roles used by this playbook [here](https://sr.ht/~fourstepper/ansible-linux-workstation/sources)

## Usage

`ansible-playbook -i inventory --diff -K playbook.yml --vault-password-file=<your_password_file>`

## Vars

See `vars/*` for inspiration and a template.

### Questions

If you have any questions, send an e-mail to the [discuss mailing list](https://lists.sr.ht/~fourstepper/ansible-linux-workstation-discuss)
