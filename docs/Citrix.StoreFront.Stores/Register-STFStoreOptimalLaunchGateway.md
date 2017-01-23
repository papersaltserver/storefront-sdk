#Register-STFStoreOptimalLaunchGateway
Register a launch Gateway with a Store
##Syntax
```
Register-STFStoreOptimalLaunchGateway [-NeverLaunchThroughGateway] <SwitchParameter> [[-FarmName] <String[]>] [[-ZoneName] <String[]>] [[-EnabledOnDirectAccess] <SwitchParameter>] [-StoreService] <StoreService> [<CommonParameters>]
```
##Detailed Description
Configure optimal NetScaler Gateway routing to optimize the handling of ICA connection routing from the HDX engine to published resources such as XenDesktop VDAs or XenApp or XenDesktop published applications using StoreFront. Typically, the optimal gateway for a site is collocated in the same geographical location. Optionally configure a farm or farms to never use a gateway, "UseNoOptimalGateway".
##Related Commands
*[Unregister-STFStoreGateway](Unregister-STFStoreGateway)
*[Register-STFStoreGateway](Register-STFStoreGateway)
*[Unregister-STFStoreOptimalLaunchGateway](Unregister-STFStoreOptimalLaunchGateway)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.Roaming.RoamingGateway
Parameter Gateway: The .NET 'Citrix.StoreFront.Model.Roaming.RoamingGateway' reference type
###System.Management.Automation.SwitchParameter
Parameter NeverLaunchThroughGateway: The .NET 'System.Management.Automation.SwitchParameter' value type
###System.String[]
Parameter FarmName: The .NET 'System.String' reference type
###System.String[]
Parameter ZoneName: The .NET 'System.String' reference type
###System.Management.Automation.SwitchParameter
Parameter EnabledOnDirectAccess: The .NET 'System.Management.Automation.SwitchParameter' value type
###Citrix.StoreFront.Model.Store.StoreService
Parameter StoreService: A .NET class representing the configuration of a StoreFront Store service
##Return Values
##Notes
When an existing Optimal gateway registration requires an update to include additional farms then it must be unregistered using UnRegister-STFStoreOptimalLaunchGateway -Gateway $gateway and then re-registered with the new list of farms / zones.