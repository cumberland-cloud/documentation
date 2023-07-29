# Terraform

## Project Structure

**Terraform** blocks are organized into files named after what they contain, e.g. _resource.tf_ will only contains `resource` blocks, _data.tf_ will only contain `data` blocks, etc. Not all projects will have every file, but all projects will _only_ have these files. 

- /.github/
    - pull_request_template.md
    - dependabot.yaml
    - /workflows/
        - action.yaml
- /docs/
    - /source/
        - /assets/
        - conf.py
        - index.rst
    - make.bat
    - Makefile
    - requirements.txt
- .gitattributes
- .gitignore
- .tfdocs.yaml
- .tflint.hcl
- .tfsec.yaml
- data.tf
- local.tf
- module.tf
- output.tf
- resource.tf
- terraform.tf
- variable.tf

**Note**: In the event that _resource.tf_ file becomes too large, it will be broken up into _resource\_\*.tf_, where the wildcard represents a logical category into which resources will be assigned, i.e. you may see,

- resource_users.tf
- resource_servers.tf
## Continuous Integration and Development