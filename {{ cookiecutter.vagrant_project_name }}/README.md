#{{ cookiecutter.vagrant_project_name }}

{{ cookiecutter.project_short_description }}

### Usage

    $ vagrant status                      # List machine(s)
    $ vagrant up [machine_name]           # Start a machine
    $ vagrant halt [machine_name]         # Stop a machine
    $ vagrant destroy [-f] [machine_name] # Destroy a machine

{% if cookiecutter.shell_provisioning != 'False' %}
### Shell provisioning

Virtual machines are provisioned executing shell scripts located in `provision` directory.
There is a variable `provision_scripts` declared in machine definition file. Provisioner will search for files which name contains the string of that variable for each machine.

{% endif %}
### Author

Create in {{ cookiecutter.year }} by {{ cookiecutter.full_name }}.

### License

{{ cookiecutter.license }}
