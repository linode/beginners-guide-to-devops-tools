# beginners-guide-to-devops-tools
An Introduction to DevOps enablement technologies. This guide will provide background information and working labs on some of the most common DevOps tools in use today. 

* [01 Introduction to CI/CD](./01-introduction-to-ci-cd.md)
* [02 Version Control](./02-version-control.md)
  * [03 GitHub](./03-github.md)
* [04 CI/CD Pipeline Automation](./04-ci-cd-automation.md)
  * [05 Jenkins](./05-jenkins.md)
* [06 Infrastructure as Code](./06-infrastructure-as-code.md)
  * [07 Terraform](./07-terraform.md)
  * [08 Ansible](./08-ansible.md)

## DevOps in a Nutshell
DevOps, a combination of **Dev**elopment and **Op**eration**s**, is as much a change in procedural mindset as it is a set of tools. Ultimately, running separate teams completely dedicated to operational tasks and software development is impractical when designing applications that have constantly growing scale and requirements. 

DevOps methods aim to speed up the cycle from idea (e.g. new feature, fix, or improvement) to development to production deployment for end user impact. This requires open and organized communication with flexible and scalable infrastructure tools. Developers are empowered with technologies focused on automation and self service to enable quick deployments for building, testing, and releasing.

![Image](https://github.com/linode/beginners-guide-to-devops-tools/blob/main/docs/assets/images/0-1.jpg)

*DevOps: Plan > Code > Build > Test > Release > Deploy > Operate > Monitor > Plan > ∞*

This guide will largely focus on Version Control for the Code/Build phases, Infrastructure as Code for the Deploy/Operate phases, and CI/CD Automation for the entire pipeline. 

*Note that many of these tools are flexable and may be used in multiple phases throughout the lifecycle.*

![Image](https://github.com/linode/beginners-guide-to-devops-tools/blob/main/docs/assets/images/0-2.jpg)

#### Additional Tools for Each Phase

- **Code/Build**: [Gitlab](https://about.gitlab.com/), [Gitea](https://gitea.io/en-us/), [Maven](https://maven.apache.org/), [Gradle](https://gradle.org/)
- **Test**: [JUnit](https://junit.org/junit5/), [Mockito](https://site.mockito.org/)
- **Deploy/Operate**:  [Salt](https://saltproject.io/), [Puppet](https://puppet.com/)
- **Monitor**:  [Prometheus](https://prometheus.io/), [Sensu](https://sensu.io/)
