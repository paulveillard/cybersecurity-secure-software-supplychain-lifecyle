#  Cybersecurity - Secure Software Supply Chain Lifecycle

An ongoing & curated collection of awesome software best practices and techniques, libraries and frameworks, E-books and videos, websites, blog posts, links to github Repositories, technical guidelines and important resources about Secure Software Supply Chain Lifecycle in Cybersecurity.
> Thanks to all contributors, you're awesome and wouldn't be possible without you! Our goal is to build a categorized community-driven collection of very well-known resources.

## `Table of Contents`


## Introduction

#### Why software security and secure supply chains matter even more today:

Digital Transformation continues at a relentless pace, putting even greater responsiblity on business executives to meet new demands of a fully customer experience. With every organization now a software-driven company, technology leaders are expected to enable business outcomes like flexibility and scale from moving to the cloud.
However, many struggle to maintain consisten security and performance in their complex, hybrid IT environment, stalling transformation efforts in their software factory.

**Organizations need integrated security tooling and processes that support DevSecOps Practices, driven in part by the following**
```
- Elevated complexity for secure development
- The growing use of open source components
- New attack vectors discovered each day
- Stricter regulatory requirements
```

## Software Supply Chain DevSecOps Challenge
The overall market is growing toward application platforms that can provide for the fast, secure, continuous deployment of great software experiences that companies compete by. But the reality is that enterprises often struggle with running these parallel tasks. Their challenges include the following:

- Maintaining and Improving legacy applications and infrastructure is complicated and places strain on already limited IT Resources
- Building and running brand new applications using modern frameworks and cloud-native application architectures increases cognitive load for dev teams
- Security is often an afterthought that's handled by security and IT operations teams at the end of the application development life cycle, with little to no collaboration with app development and other teams.
- Disparate application security and DevOps tools, practices and disjointed processes result in tool sprawl; this impedes collaboration, visibility, and productivity and increases the change of human error.

DevSecOps Best Practices for Developers:

- Implement Security Early and Often
- Automate Security Wherever Possible
- Emphasize Collaboration between development, security, and operations teams
- Use secure coding practices
- Conduct regular security assessments
- Continuously monitor and improve security

## Enabling a successful DevSecOps Practice
Successfully implementing DevSecOps begins well before the application pipeline. As a first step, organizations will want to ensure their underlying infrastructure and application services are running on an enterprise open source foundation prehardened with built-in security tools and features.
### 1) Get trusted images and libraries out-of-the-box

- **Stay on top of the latest vulnerabilities and security risks** by making use of trusted content in the form of libraries from popular application frameworks available including Java, Node.js, Python, Go, and packages from Red Hat Enterprise Linux (RHEL).

### 2)  Maintain a highly available container registry from which to securely access and incorporate attested, curated packages

- **Restrict access to the container registry and the images stored** within using granular role-based access controls (RBAC) to reduce risk of unauthorized entry. 
- **Securely store and manage images that are used to deploy applications and services**, ensuring that only trusted images are used in production. 
- **Run rootless container images to install packages and run services safely** within the container without impacting the host.
- **Increase transparency and visibility across software factories** to build trust between security teams and DevOps teams.
- **Allow image signing for verification and authentication,** which helps prevent malicious code from being added to the registry.
- **Verify the authenticity of the software build of materials** and prevent tampering to ensure code integrity.
- **Support the use of digital signatures and certificates** that attests to the origin of software components as coming from a trusted source.


