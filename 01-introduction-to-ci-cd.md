## Introduction to CI/CD
A key component of DevOps is a **C**ontinuous **I**ntegration and **C**ontinuous **D**eployment (CI/CD). CI/CD pipelines are designed to improve software delivery by automating steps for building, testing, production, and monitoring of the software development lifecycle. This enables teams to develop code faster and more reliably while bringing development and operational teams together.


![Image](https://github.com/linode/beginners-guide-to-devops-tools/blob/main/docs/assets/images/1-1.jpg)


### What is Continuous Integration?
In software development, integration is the process of incorporating changes like refactored code, new features, or bug fixes into the existing codebase.

Traditionally, integration is performed in preparation of the deployment of a new release. This approach can lead to problems, as integrating multiple or large changes in one go may result in last-minute conflicts and bugs. Several strategies have emerged to mitigate these problems. Continuous Integration (CI) is one such solution: it creates a workflow where every commit made to the codebase is tested and built, and each developer on the project is expected to commit code at least once per day. Usually, both testing and building are automated, so that every commit to the central repository triggers an automatic build. If the build is successful, it triggers a run of the test suite. This way, conflicts or bugs are discovered quickly over the course of development, making the release process smoother and less painful.

### What is Continuous Delivery?
Continuous Delivery (CD) takes the principle of CI one step further: the automated build and test process is extended to every component of the application, including configuration files, database schemas, and environments. Whenever changes are made to any of these components, the build and test procedure is performed (ideally through an automated pipeline) so that the resulting build can be easily deployed. The resulting build does not always have to be released to production, but it should at least be deployed to an environment (such as staging) that is as close to production as possible. Product owners can therefore be confident that any build that makes it through this pipeline is releasable to the public. This approach offers several advantages:

Traditionally, integration is performed in preparation of the deployment of a new release. This approach can lead to problems, as integrating multiple or large changes in one go may result in last-minute conflicts and bugs. Several strategies have emerged to mitigate these problems. Continuous Integration (CI) is one such solution: it creates a workflow where every commit made to the codebase is tested and built, and each developer on the project is expected to commit code at least once per day. Usually, both testing and building are automated, so that every commit to the central repository triggers an automatic build. If the build is successful, it triggers a run of the test suite. This way, conflicts or bugs are discovered quickly over the course of development, making the release process smoother and less painful.

* New features and bug fixes can move from concept to deployment faster.
* Because the difference between each release is small, the risk of an individual deployment breaking is reduced.
* For the same reason, it is easier and safer to revert to a previous version in the event of an issue.
* As with continuous integration, continually building and testing environments and configuration parameters means that problems are discovered earlier in the development process.

### Pipelines
Pipelines are an important concept in CI/CD. A pipeline is a sequence of steps that will be run whenever a change is made to a project (source code, database schemas, environments, or configuration). Pipelines can include steps executed in series or in parallel, and often multiple pipelines are used to handle different situations when working on a project.


![Image](https://justin-test.us-east-1.linodeobjects.com/placeholder.png)

This example illustrates a continuous delivery pipeline. When code is committed to the staging branch, it is built and tested on the CI server as before. This time, tests are run on different browsers for a more production-ready test environment. The environments are also dockerized, which helps guarantee that all developers will be working in identical environments and makes differences between production, staging, and test environments explicit. If these steps complete successfully, the build is then deployed to the staging branch.
