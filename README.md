# Development bootstrap with Ansible to Ubuntu

## Requeriments

Make sure that you have been installed the Ansible.

    sudo apt install ansible

## How to use

Command to Install all.

    sudo ansible-playbook site.yml

Command to install a specific role

    sudo ansible-playbook site.yml --tags "<tag_name>"

Like that...

    sudo ansible-playbook site.yml --tags base-bootstrap

    sudo ansible-playbook site.yml --tags java11-oracle

or multiple tags

    sudo ansible-playbook site.yml --tags git,java11-oracle,chrome

## Avaliables Roles & tags

- { role: 'indicator-multiload', tags: ['base-bootstrap', 'indicator-multiload']}
- { role: 'git', tags: ['base-bootstrap', 'git']}
- { role: 'vs-code', tags: ['base-bootstrap', 'vs-code']}
- { role: 'docker', tags: 'docker'}
- { role: 'java8-oracle', tags: 'java8-oracle'}
- { role: 'java11-oracle', tags: 'java11-oracle'}
- { role: 'openjdk-11', tags: 'openjdk-11'}
- { role: 'node-js', tags: 'nodejs'}
- { role: 'angular-cli', tags: 'angular-cli'}
- { role: 'intellij', tags: 'intellij'}
- { role: 'chrome', tags: 'chrome'}
- { role: 'skypeforlinux', tags: 'skype'}

## How create a new role

1. Navigate to the role directory `cd /roles`
2. Create the new role using the command `ansible-galaxy init`
3. Change the 'task' todo whenerever that you want in `/tasks/main.yaml` and anything more necessary
4. Add the new role with the properly tags in the `site.yaml` in the root directory
5. Enjoy :)

### TODO/WIP

- eclipse
- Double check and refactoring of all
