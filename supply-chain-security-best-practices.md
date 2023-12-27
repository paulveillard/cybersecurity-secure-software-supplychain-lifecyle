# Supply Chain Security Best Practices: How to Protect Containerized Applications

Managing today’s software — composed of a combination of open source code, in-house code, and third-party code — has elevated the application risk from design and build through production and management. With more points of vulnerability within today’s software supply chain, the number of attacks has grown exponentially.

> It’s not enough anymore to simply run security tests at the end of the development and production process. Waiting that long can have a huge negative impact on your business. In the cloud native era, security needs to be a focal point throughout production and the entire application life cycle.


## `Table of Contents`
- [Supply Chain Functional Definition](#)
- [Secure Supply Chain Assessment](#)

## `A functional definition of what software supply chain security is.`
Vulnerabilities can occur at all stages of the software life cycle.

![image](https://github.com/paulveillard/cybersecurity-secure-software-supplychain-lifecyle/blob/main/img/supply-chain-attacks.PNG)


In the cloud native era, properly securing the **software supply chain starts at the very beginning of the development process and continues throughout production and the entire application life cycle. The tradition of implementing security tests at the end of the development and production process or patching running applications is outmoded.**

> Improper security implementation can seriously impact business by delaying important releases in order to address issues found later in the software life cycle or by losing security fixes that were only applied to running workloads.


Just as automation is key for Kubernetes, it’s also critical for the software supply chain. Proper security is continuous, with security gates implemented throughout the build, deploy and runtime process. Proper security allows developers to do their work with guidance from security policies implemented with automated tools that analyze, monitor and intervene when things go awry.


##  `How to assess the threat landscape.`

DevOps teams are well aware of the ubiquity of code vulnerabilities that find their way into the development pipeline and in production — but how attackers are exploiting bad code is getting worse.

![image-3](https://github.com/paulveillard/cybersecurity-secure-software-supplychain-lifecyle/blob/main/img/supply_chain_3.PNG)


### Supply Chain Automation Best Practices

In order To Start locking down the supply chain and protect applications and code. These best practices include the automation of:

- Analysis of code from all sources before the development process even begins, with a software bill of materials (SBOM) for each code source. The SBOM should come with any code that is used. For code and application distribution, open source alternatives such as the Software Package Data Exchange (SPDX) serve to communicate SBOMs.

- Adherence to the supply-chain levels for software artifacts, or SLSA (pronounced “salsa”).

- The integration of policy checks through CI/CD and in runtime.

- Container image scanning before an image is pulled into the build and before deployment.

- Signing tools, such as Sigstore, for signing images and configuration files.

- Continuous audit and logging for each step in the supply chain.

- Role-based access and authorization control for all tools used in the supply chain and in production, including namespace and other access to Kubernetes clusters.

- Collection and analysis of platform audit logs, and application logging and monitoring for potential security issues.

- Runtime behavioral security analysis for detection of anomalous behavior.

- Processes that ensure that information discovered during development informs deployment and production policies, and that information discovered in production is fed back into the development process.


##  `Where and how to get started with supply chain security. `
#### What are SBOMs?
The “shift left” trend is generally thought to apply to the very beginning of the development cycle, at the point when developers first begin to create code and make pull requests. However, for a trusted software supply chain, the work needs to begin in the open source projects that are the building blocks for custom applications.

 

The information that an SBOM provides about an application, a code library or a third-party vendor’s software is often compared to the lists of ingredients and additives listed on a food label. 

An SBOM provides a library of all libraries used in an application, with a history of all code sources and timelines.

#### What is SLSA?
The SLSA framework was designed for organizations to make use of its guidance gradually. It is designed to be adopted in incremental steps, all of which offer tangible improvement for software supply chain security along the way. SLSA includes four levels, or “milestones,” as they are called in the documentation, that organizations can attain.


##  `Secure Supply Chain Assessment`

So we have laid down a blueprint for supply chain security — the things your
organization needs to keep its software safe at all stages of its life cycle.
This includes software provenance with SBOMs and SLSA. We saw how
GitOps represents a cornerstone for DevSecOps. We also reviewed the management and
support of supply chain security best practices as code, thanks to its reliance on
versioning and traceability, along with the audit trails it supports, and other benefits
for cloud native environments.

### Evaluating your supply chain security
#### A framework for supply chain evaluation
So how does your supply chain stack up? Here are some questions to ask yourself:

## Verify source code
- Do you require signed commits?

Do you use git hooks or automated scans to prevent committing secrets to source control?

Have you defined an unacceptable risk level for vulnerabilities? For example: no code may be committed that includes Critical or High vulnerabilities

Do you use automated scanning to detect and prevent security issues, vulnerable dependencies, etc. from being committed to the repo that are not in compliance with your defined risk threshold?

Have you defined clear contributors roles? Are they documented and discoverable?

Do you enforce review and approval of contributions prior to merging?

Are branch protection rules in place?

Do you enforce MFA and SSH keys for human-entities? Do you have a plan in place for rotating SSH keys at regular intervals or following a key leak?

Do you limit the access of automation agents (like CI/CD pipelines) following the principles of least privilege and just-in-time?

## Verify materials
- Do you verify that dependencies meet your minimum thresholds for quality and reliability?

- Do you automatically scan dependencies for security issues and license compliance?

- Do you automatically perform Software Composition Analysis on dependencies when they are downloaded/installed?

- Do you monitor dependencies for updates and security issues?

- Do you build dependencies yourself instead of relying on public package managers?

- Do you create an SBOM of your own artefacts?

## Protecting build pipelines
- Do you use hardened, minimal containers as the foundation for your build workers?

- Do you maintain your build and test pipelines as Infrastructure-as-Code?

- Do you automate every step in your build pipeline outside of code reviews and final sign-offs?

- Do you sign the output of every step in your build pipeline to provide a verifiable guarantee?

- Do you validate the signatures and checksums of all dependencies before ingesting them in a build stage?

- Do you use separate build workers/containers for each step in your build pipeline?

- Do your pipeline orchestrator pass in the environments, tools, and commands allowed on each build worker?

- Do you network isolate your build workers and pipeline as much as possible?

- Do you produce verifiable, reproducible builds?

## Protecting artefacts and deployments
- Is every artefact you produce (including metadata and intermediate artefacts) signed?

- Do you distribute metadata in a way that can be verified by downstream consumers of your products?

- Can your downstream consumers verify/validate any artefact they ingest from you before they use/deploy it?


## How to defend your software throughout its full life cycle.
