# Satellite 6.2 Host Move Playbook for Ansible

This workflow is built to assist administrators with the migration of a Satellite-managed host to a different capsule in the same Satellite environment

## Getting Started

Currently the workflow is shipped as an Ansible playbook.  Simply clone the repo and run the playbook on a host pointing to your Satellite environment

### Prerequisities

Ansible control system with SSH access to the Satellite 6.2 Target
Environment with multiple capsule servers (included the embedded Capsule in Satellite itself)
A valid Satellite 6 subscription on access.redhat.com

### Running the playbook

Run the playbook as follows:

```
ansible-playbook -i hosts satellite62-install.yaml --extra-vars ""
```

## Built With

* Ansible
* Hammer CLI for Satellite configuration

## Authors

* **Tim Fairweather** - *Initial work*
