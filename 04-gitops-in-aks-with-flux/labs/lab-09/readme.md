# lab-09 - Cleaning up

## Estimated completion time - 10 min

To avoid Azure charges, you should clean up unneeded resources. When the clusters are no longer needed, use the `az group delete` command to remove the ACR, AKS, resource groups and all related resources.

## Goals

* Cleanup unused resources to avoid unnecessary costs

## Task #1 - delete clusters and supported resources

When you are done, delete both resource groups.

```bash
# Delete blue cluster
az group delete -g iac-ws4-blue-rg -y

# Delete green cluster
az group delete -g iac-ws4-green-rg -y

# Delete red cluster
az group delete -g iac-ws4-red-rg -y

# Delete shared resources
az group delete -g iac-ws4-rg -y
```
## Useful links

* [az group delete](https://docs.microsoft.com/en-us/cli/azure/group?view=azure-cli-latest&WT.mc_id=AZ-MVP-5003837#az_group_delete)