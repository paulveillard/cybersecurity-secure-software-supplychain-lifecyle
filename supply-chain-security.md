# Supply Chain Security: How to Protect Containerized Applications

Managing today’s software — composed of a combination of open source code, in-house code, and third-party code — has elevated the application risk from design and build through production and management. With more points of vulnerability within today’s software supply chain, the number of attacks has grown exponentially.

> It’s not enough anymore to simply run security tests at the end of the development and production process. Waiting that long can have a huge negative impact on your business. In the cloud native era, security needs to be a focal point throughout production and the entire application life cycle.


## `Table of Contents`

## `A functional definition of what software supply chain security is.`
Vulnerabilities can occur at all stages of the software life cycle.

![image](https://github.com/paulveillard/cybersecurity-secure-software-supplychain-lifecyle/blob/main/img/supply-chain-attacks.PNG)


In the cloud native era, properly securing the **software supply chain starts at the very beginning of the development process and continues throughout production and the entire application life cycle. The tradition of implementing security tests at the end of the development and production process or patching running applications is outmoded.**

> Improper security implementation can seriously impact business by delaying important releases in order to address issues found later in the software life cycle or by losing security fixes that were only applied to running workloads.


Just as automation is key for Kubernetes, it’s also critical for the software supply chain. Proper security is continuous, with security gates implemented throughout the build, deploy and runtime process. Proper security allows developers to do their work with guidance from security policies implemented with automated tools that analyze, monitor and intervene when things go awry.


## How to assess the threat landscape.
Supply Chain Automation Best Practices

In order To Start locking down the supply chain and protect applications and code. These best practices include the automation of:

Analysis of code from all sources before the development process even begins, with a software bill of materials (SBOM) for each code source. The SBOM should come with any code that is used. For code and application distribution, open source alternatives such as the Software Package Data Exchange (SPDX) serve to communicate SBOMs.

Adherence to the supply-chain levels for software artifacts, or SLSA (pronounced “salsa”).

The integration of policy checks through CI/CD and in runtime.

Container image scanning before an image is pulled into the build and before deployment.

Signing tools, such as Sigstore, for signing images and configuration files.

Continuous audit and logging for each step in the supply chain.

Role-based access and authorization control for all tools used in the supply chain and in production, including namespace and other access to Kubernetes clusters.

Collection and analysis of platform audit logs, and application logging and monitoring for potential security issues.

Runtime behavioral security analysis for detection of anomalous behavior.

Processes that ensure that information discovered during development informs deployment and production policies, and that information discovered in production is fed back into the development process.


## Where and how to get started with supply chain security.


## The full checklist of best practices.


## How to defend your software throughout its full life cycle.
