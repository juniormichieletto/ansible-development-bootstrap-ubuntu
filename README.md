# Development bootstrap with Ansible to Ubuntu

## Requeriments

Make sure that you have been installed the Ansible.

Download in: www.ansible.com

## Hand-on

Command to Install all.

`
    ansible-playbook -l localhost playbook.yml
`

Command to install a specific role

`
    ansible-playbook -l localhost playbook.yml --tags "<tag_name>"
`

## Avaliables Roles & tags:

- { role: 'git', tags: 'git'}
- { role: 'docker', tags: 'docker'}
- { role: 'java8-oracle', tags: 'java8-oracle'}
- { role: 'node-js', tags: 'nodejs'}
- { role: 'angular-cli', tags: 'angular-cli'}
- { role: 'vs-code', tags: 'vs-code'}
- { role: 'intellij', tags: 'intellij'}
- { role: 'chrome', tags: 'chrome'}
- { role: 'skypeforlinux', tags: 'skype'}

### TODO/WIP

- jdk-10 (maybe a select over var)
- jdk-11 (maybe a select over var)
- eclipse
- Double check and refactoring of all