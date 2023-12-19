# Enable Modules

To use a Kyma module, you must enable it first. Use Kyma dashboard or Kyma CLI to do that. If you don't need the module anymore, disable it to save resources.

Enable and Disable a Kyma Module Using Kyma Dashboard
Use Kyma dashboard to enable and disable a Kyma module in the release channel of your choice.

Context
If there are no modules enabled on your cluster, you can easily enable one from the Cluster Details view. Select Add Module and follow the wizard steps.

If you want to enable additional modules, follow this procedure:

Procedure
Log in to Kyma dashboard. The URL is in the Overview section of your subaccount.
Go to the kyma-system Namespace.
In the Kyma section, choose the Kyma resource.
Select your Kyma instance (default) and choose Edit.
In Kyma Default Channel, you can change the release channel for all your modules at the Kyma custom resource (CR) level, or keep the default one.
Note
By default, Kyma modules are part of the regular channel. It allows for delivering the modules at a slower, predictable rate for production environments with minimal disturbance. You can change to the fast channel for a more fluid release process that offers the latest technical updates and features at a quicker pace. For more information about the release channels, see Kyma Release Channels.

In the Modules section, check the modules you want to enable.
Optional: At the module level, you can overwrite the release channel for the current module by choosing the available channel.
Select Update.
Results
This process may take a while, depending on the number of modules. The operation was successful when the module status changes to READY
