## Infrastructure as Code
Infrastructure as Code (IaC) is a philosophy and a set of practices for breaking down the deployment and managing systems and networks into portable blocks of code. The fully automated installation and configuration provided by these tools allows the DevOps teams to define complete systems with configuration files.

Configuration files are sets of instructions with specifications on how to assemble and configure the system. This instruction set can take many different forms and go by other names depending on the tool (e.g., a cookbook in Chef and a playbook in Ansible). Regardless of the differences between platforms, this ability to define a complete configuration in advance leads to a new vision of infrastructure, in which knowledge of the systems resides in code form, and gets rapidly deployed without the need for conventional installation or reconfiguration with console commands.

IaC plays an important role in enabling DevOps practices and CI/CD pipelines by removing the majority of provisioning work from developers. Teams running IaC can quickly launch scripts to have their infrastructure up and running new versions of their applications while sidestepping potential bottlenecks from traditional methods deployment methods.

IaC also enables consistency through every step as Infrastructure will move through the same CI/CD pipeline as an application and can be tested along with the application.

* [06 Infrastructure as Code](./06-infrastructure-as-code.md)
  - [07 Terraform](07-terraform.md)
  - [08 Ansible](08-ansible.md)
