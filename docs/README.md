# Overview

![Crossplane](media/banner.png)

Crossplane is an open source Kubernetes add-on that extends any cluster with
the ability to provision and manage cloud infrastructure, services, and
applications using kubectl, GitOps, or any tool that works with the Kubernetes
API.

With Crossplane you can:

* **Provision & manage cloud infrastructure with kubectl**
  * [Install Crossplane] to provision and manage cloud infrastructure and
    services from any Kubernetes cluster.
  * Provision infrastructure primitives from any provider ([GCP], [AWS],
    [Azure], [Alibaba], on-prem) and use them alongside existing application
    configurations.
  * Version, manage, and deploy with your favorite tools and workflows that
    you’re using with your clusters today.

* **Publish custom infrastructure resources for your applications to use**
  * Define, compose, and publish your own [infrastructure resources] with
    declarative YAML, resulting in your own infrastructure CRDs being added to
    the Kubernetes API for applications to use.
  * Hide infrastructure complexity and include policy guardrails, so
    applications can easily and safely consume the infrastructure they need,
    using any tool that works with the Kubernetes API.
  * Consume infrastructure resources alongside any Kubernetes application to
    provision and manage the cloud services they need with Crossplane as an
    add-on to any Kubernetes cluster.

* **Deploy applications using a team-centric approach with OAM**
  * Define cloud native applications and the infrastructure they require with
    the Open Application Model ([OAM]).
  * Collaborate with a team-centric approach with a strong separation of
    concerns:
    * Infrastructure operators - provide infrastructure and services for
      applications to consume
    * Application developers - build application components independent of
      infrastructure
    * Application operators - compose, deploy, and run application
      configurations
  * Deploy application configurations from app delivery pipelines or GitOps
    workflows, using the proven Kubernetes declarative model.

## Getting Started
[Install Crossplane] into any Kubernetes cluster to get started.

## Mission

Crossplane strives to be the best Kubernetes add-on to provision and manage the
infrastructure and services your applications need directly from kubectl. A
huge part of this mission is arriving at an elegant, flexible way to define,
compose, and publish your own infrastructure resources to the Kubernetes API
and to model and manage cloud native applications.

The path of cloud native apps from developer laptop into production requires
collaboration across teams to build the app itself, deploy and manage the app
and it’s infrastructure, and publishing infrastructure resources that embody
organizational best practices and security policies.

Today, multiple tools and management models must be glued together in
deployment pipelines that are often fragile and error prone. Teams can find it
difficult to collaborate in an effective way when aspects of an application are
blurred, resulting in a lack of clear ownership and conflicts integrating
changes. Requiring team members to master multiple tools, languages, and
philosophies, while understanding the interactions and failure modes between
them can significantly impede an organization’s ability to deliver applications
efficiently.

Crossplane believes that a team-centric approach with a strong separation of
concerns combined with the proven Kubernetes declarative model is the best way
to provision and manage infrastructure and cloud native applications. Teams
should be able to publish infrastructure resources for applications to consume,
define application components independent of infrastructure, and compose both
into complete application configurations -- all using declarative YAML that can
be deployed with kubectl from app delivery pipelines or with GitOps workflows.

This team-centric approach reflects individuals often specializing in the
following roles:

*   **Infrastructure Operators** - provide infrastructure and services for apps
    to consume
*   **Application Developers** - build application components independent of
    infrastructure
*   **Application Operators** - compose, deploy, and run application
    configurations

This separation of concerns is core to Crossplane’s approach to infrastructure
and application management, so team members can deliver value by focusing on
what they know best.

With Crossplane, infrastructure operators can define custom infrastructure
resources with declarative YAML and publish them for applications to consume
as Kubernetes custom resources or with any tool that works with the Kubernetes
API. These infrastructure resources can be used with existing Kubernetes
applications (Deployments, Services) and with application definition models
like OAM.

The result is a consistent, integrated, and modular approach to managing
infrastructure and application configurations, that can be deployed with the
same tooling including kubectl, GitOps, and anything can talk with the
Kubernetes API.

<!-- Named Links -->

[Install Crossplane]: getting-started/install.md
[Custom Resource Definitions]: https://kubernetes.io/docs/concepts/extend-kubernetes/api-extension/custom-resources/
[reconciling]: https://kubernetes.io/docs/concepts/architecture/controller/
[GCP]: https://github.com/crossplane/provider-gcp
[AWS]: https://github.com/crossplane/provider-aws
[Azure]: https://github.com/crossplane/provider-azure
[Alibaba]: https://github.com/crossplane/provider-alibaba
[infrastructure resources]: https://blog.crossplane.io/crossplane-v0-10-compose-and-publish-your-own-infrastructure-crds-velero-backup-restore-compatibility-and-more/
[OAM]: https://github.com/oam-dev/spec/releases/tag/v1.0.0-alpha.2
