#  Cybersecurity - Secure Software Supply Chain Lifecycle: Theory, Techniques, and Tools

An ongoing & curated collection of awesome software best practices and techniques, libraries and frameworks, E-books and videos, websites, blog posts, links to github Repositories, technical guidelines and important resources about Secure Software Supply Chain Lifecycle in Cybersecurity.
> Thanks to all contributors, you're awesome and wouldn't be possible without you! Our goal is to build a categorized community-driven collection of very well-known resources.

# Theory
## Therory `Table of Contents`
- [Introduction](#)
- [Enabling a successful DevSecOps Practice](#)
  - [Get trusted images and libraries out-of-the-box](#1-get-trusted-images-and-libraries-out-of-the-box)
  - [Maintain a highly available container registry from which to securely access and incorporate attested, curated packages](#2--maintain-a-highly-available-container-registry-from-which-to-securely-access-and-incorporate-attested-curated-packages)

## Tools - Table of Contents
- [software-supply-chain-security - Tools](#software-supply-chain-security-tools)
  - [Introduction - What](#introduction)
  - [Dependency intelligence](#dependency-intelligence)
    - [SCA and SBOM](#sca-and-sbom)
    - [Vulnerability information exchange](#vulnerability-information-exchange)
  - [Point-of-use validations](#point-of-use-validations)
    - [Supply chain beyond libraries](#supply-chain-beyond-libraries)
  - [Identity, signing and provenance](#identity-signing-and-provenance)
  - [Frameworks and best practice references](#frameworks-and-best-practice-references)
  - [Build techniques](#build-techniques)
  - [Talks, articles, media coverage and other reading](#talks-articles-media-coverage-and-other-reading)
    - [Getting started and staying fresh](#getting-started-and-staying-fresh)



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


#### Elevated complexity for secure development
#### The growing use of open source components
#### New attack vectors discovered each day
#### Stricter regulatory requirements

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

## Enabling a Successful DevSecOps Practice
Successfully implementing DevSecOps begins well before the application pipeline. As a first step, organizations will want to ensure their underlying infrastructure and application services are running on an enterprise open source foundation prehardened with built-in security tools and features.

> Developers need security scanning and guidance across all aspects of cloud-based applications. Beyond just the software packages, they need security coverage on tooling, application configurations, and the entire solution architecture, including infrastructure.

> Developers also need flexibility to move workloads to any footprint that works best with consumption options to match the organization’s needs for an open hybrid cloud. Building on trusted, industry-proven container orchestration platforms adds the advantages of standards and consistency to continue their investments in, for example, a Kubernetes-native Java framework like Quarkus.



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

### 3) Protect source code and dependencies in code management with security best practices
- Analyze and detect potential vulnerabilities, malware, or other malicious code before they are consumed across software factories.
- Make use of automated code analysis to scan for potential security vulnerabilities in images and for other security issues before they’re committed to the code repository.
- You need to carefully manage dependencies, and any libraries or components used in the build process should be regularly audited for vulnerabilities.
- Component analysis helps organizations identify and assess the risk of third-party components in their software supply chain.

### 4) Strengthen the CI/CD pipeline with an automated chain of trust and approval gates
- Control the flow of software dependencies and ensure that only trusted packages are used in builds and deployments to prevent poisoned pipeline execution in the software factory.
- Manage and secure the use of various software components that make up the build by first auto-generating software bill of materials (SBOMs) with metadata on how each artifact was built.
- Authenticate provenance to industry standards through version control, auditing, and traceability of all software components used in the development process.
- Automate CI/CD pipelines with regular security checks integrated throughout the build process to ensure all inputs and outputs are secure as teams compile code, build images, and run tests.
-  Institute strong protections against tampering through cross-build contamination.
-  Immediately detect and alert on any changes or unauthorized modifications to the source code and OSS dependencies that are impacting build artifacts stored in the repository.
- Determine which versions of what components were used in any given application and understand the impact of that change to mitigate risks in the SDLC.


### 5) Monitor applications at runtime with contextual insights into vulnerabilities and threats to deployed workloads
- Ensure that deployment environments are secure at runtime by implementing proper access controls, threat prevention and anomaly detection, network segmentation, and runtime vulnerability detection.
- Provide complete end-to-end visibility into all components and their respective sources to continuously monitor and proactively identify changes in the risk profile caused by malicious components.
- Implement monitoring and logging systems that instantly detect, alert, and direct on potential security incidents.

# Tools

## Table of Contents
- [software-supply-chain-security - Tools](#software-supply-chain-security-tools)
  - [Introduction - What](#introduction)
  - [Dependency intelligence](#dependency-intelligence)
    - [SCA and SBOM](#sca-and-sbom)
    - [Vulnerability information exchange](#vulnerability-information-exchange)
  - [Point-of-use validations](#point-of-use-validations)
    - [Supply chain beyond libraries](#supply-chain-beyond-libraries)
  - [Identity, signing and provenance](#identity-signing-and-provenance)
  - [Frameworks and best practice references](#frameworks-and-best-practice-references)
  - [Build techniques](#build-techniques)
  - [Talks, articles, media coverage and other reading](#talks-articles-media-coverage-and-other-reading)
    - [Getting started and staying fresh](#getting-started-and-staying-fresh)


## License
MIT License & [cc](https://creativecommons.org/licenses/by/4.0/) license

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.

To the extent possible under law, [Paul Veillard](https://github.com/paulveillard/) has waived all copyright and related or neighboring rights to this work.

