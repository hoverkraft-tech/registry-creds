## Roadmap & status

The primary purpose of this tool is to ease the every-day lives of developers and new-comers to Kubernetes. When you move to production, you can use something like Flux, Argo or Terraform (see appendix) for managing secrets across namespaces.

Disclaimer: see the [license of this project](/LICENSE) before deploying or using it.

You can create a test cluster very quickly with something like [KinD](https://kind.sigs.k8s.io/docs/user/quick-start/) to try it out.

Todo:
- [ ] Remove pull secret reference from ServiceAccounts upon ClusterPullSecret deletion
- [ ] Propagate alterations/updates to the primary `ClusterPullSecret` in each namespace when the secret value changes (the work-around is to delete and re-create the ClusterPullSecret)
