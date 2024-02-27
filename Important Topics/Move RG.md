## Reorganize Azure resources

Sometimes you may need to move resources to either a new subscription or a new resource group in the same subscription.

![image](https://github.com/rafid29mehda/AZ-104/assets/71279591/2a8c2ec5-40c3-4f84-9b86-6dc69aea441d)

When moving resources, both the source group and the target group are locked during the operation. Write and delete operations are blocked on the resource groups until the move completes. This lock means you can't add, update, or delete resources in the resource groups. Locks don't mean the resources aren't available. For example, if you move a virtual machine to a new resource group, an application can still access the virtual machine.

### Limitations
Before beginning this process be sure to read the Move operation support for resources page. This page details what resources can be moved between resources group, subscriptions, and regions.

### Implementation
To move resources, select the resource group containing those resources, and then select the Move button. Select the resources to move and the destination resource group. Acknowledge that you need to update scripts.

![image](https://github.com/rafid29mehda/AZ-104/assets/71279591/d537b1c6-3717-4d4c-8678-cb031bc85dc6)


 ### Note

Just because a service can be moved doesn’t mean there aren’t restrictions. For example, you can move a virtual network, but you must also move its dependent resources, like gateways.
