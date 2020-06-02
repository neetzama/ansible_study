# Automation of middleware installation and various settings by Ansible.
It aims to automate the construction of the infrastructure environment.<br>
But I'm only talking about Ansible here.<br>
[Click here][1] for an overview of the entire project.<br>
```
├── hosts
├── playbook.yml
├── roles
│   ├── apt
│   │   └── tasks
│   │       └── main.yml
│   ├── gunicorn
│   │   ├── tasks
│   │   │   └── main.yml
│   │   └── templates
│   │       ├── gunicorn.service.j2
│   │       └── gunicorn.socket.j2
│   ├── nginx
│   │   ├── tasks
│   │   │   └── main.yml
│   │   └── templates
│   │       └── config.j2
│   ├── postgresql
│   │   └── tasks
│   │       └── main.yml
│   └── venv
│       ├── handlers
│       │   └── main.yml
│       ├── tasks
│       │   └── main.yml
│       └── templates
└── vars
    ├── main.yml
    └── private.yml
```
- Use Ansible to automate the middleware and various settings required for the django application
- The directory structure is as shown above.
- The details of the resources to be tested are [listed here][2]
## Requirement
- ansible 2.9.5
- Python 3.6.9
- Django==3.0.3
- nginx 1.14.0
- gunicorn 20.0.2

[1]: https://github.com/neetzama/jenkins_study
[2]: https://github.com/neetzama/cloudformation_study