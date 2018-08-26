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
- { role: 'java8-oracle', tags: 'java8-oracle'}
- { role: 'vs-code', tags: 'vs-code'}
- { role: 'chrome', tags: 'chrome'}
- { role: 'skypeforlinux', tags: 'skype'}

### TODO/WIP

- Docker
- Docker-compose
- Nodejs
- Angular-CLI
- jdk-10 (maybe a select over var)
- jdk-11 (maybe a select over var)
- Intellj
- eclipse
- Double check and refactoring of all