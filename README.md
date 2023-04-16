# Ansible Execution Environment

## Ansible Builder
cd execution
ansible-builder build
```sh
Running command:
  docker build -f context/Dockerfile -t ansible-execution-env:latest context
Complete! The build context can be found at: ./context
```

## Ansible Navigator
ansible-navigator run ../playbooks/azure_info.yml --eei ansible-execution-env:latest
```sh
---------------------------------------------------------------
Execution environment image and pull policy overview
---------------------------------------------------------------
Execution environment image name:     ansible-execution-env:latest
Execution environment image tag:      latest
Execution environment pull arguments: None
Execution environment pull policy:    tag
Execution environment pull needed:    True
---------------------------------------------------------------
Updating the execution environment
---------------------------------------------------------------
Running the command: docker pull ansible-execution-env:latest
```