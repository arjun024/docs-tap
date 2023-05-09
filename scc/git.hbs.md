# Use Git with Supply Chain Choreographer

This topic explains how you can use Git with Supply Chain Choreographer.

The out of the box supply chains and delivery use Git in 3 ways:

- To fetch the developers source code, using the [template](ootb-template-reference.hbs.md#source-template).
- To store complete Kubernetes configuration, the "write" side of gitops, use 
  [template 1](ootb-template-reference.hbs.md#config-writer-template) and [template 2](ootb-template-reference.hbs.md#config-writer-and-pull-requester-template).
- To fetch stored Kubernetes configuration, the read side of gitops,
  from either the same or a different Kubernetes cluster, use the
  [template](ootb-template-reference.hbs.md#delivery-source-template).

## Supported Git Repositories

Tanzu Application Platform supports two Git providers:

- GitHub
- GitLab

## Related Articles

[Git Authentication](git-auth.hbs.md): walks through the objects, such as secrets and service accounts,
to create on cluster to allow supply chain Git operations to succeed.

[GitOps versus RegistryOps](gitops-vs-regops.hbs.md): discusses the two methods of storing built Kubernetes
configuration, either in a git repository or an image registry, and walks through the parameters that must
be provided for each.
