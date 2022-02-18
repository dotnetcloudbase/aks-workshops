# lab-09 - Cleaning up

## Estimated completion time - 10 min

To avoid Azure charges, you should clean up unneeded resources. When the cluster is no longer needed, use the az group delete command to remove the ACR, AKS, resource group and all related resources.

## Goals

* Cleanup unused resources to avoid unnecessary Azure costs

## Task #1 - delete the cluster

When you are done, delete both resource groups.

```bash
# Delete dev-blue resource group
az group delete -n iac-dev-blue-rg --yes

# Delete dev-blue resource group
az group delete -n iac-dev-green-rg --yes

# Delete base resource group
az group delete -n iac-dev-rg --yes
```

## Useful links

* [az group delete](https://docs.microsoft.com/en-us/cli/azure/group?view=azure-cli-latest&WT.mc_id=AZ-MVP-5003837#az_group_delete)
