#Add-STFStoreService
Creates a new StoreFront Store Service at the supplied IIS VirtualPath and optional SiteId.
##Syntax
```
Add-STFStoreService [-Anonymous] <SwitchParameter> [-VirtualPath] <String> [[-SiteId] <Int64>] [[-FarmName] <String>] [[-FarmType] <XenApp | XenDesktop | AppController | VDIinaBox>] [[-Servers] <String[]>] [[-Port] <Int32>] [[-TransportType] <HTTP | HTTPS | SSL>] [[-SSLRelayPort] <Int32>] [[-LoadBalance] <Boolean>] [[-AllFailedBypassDuration] <Int32>] [[-BypassDuration] <Int32>] [[-FriendlyName] <String>] [[-Zones] <String[]>] [[-ConnectionString] <String>] [<CommonParameters>]
```
##Detailed Description
StoreFront stores aggregate desktops and applications, making them available to users. Stores appear in Citrix Receiver under users' accounts, so choose a VirtualPath that gives users information about the content of the store.
##Related Commands
*[Get-STFStoreService](Get-STFStoreService)
*[Remove-STFStoreService](Remove-STFStoreService)
*[Set-STFStoreService](Set-STFStoreService)
##Parameters
|Name|Description|Required?|Pipeline Input|
###System.String
Parameter VirtualPath: The .NET 'System.String' reference type
###System.Int64
Parameter SiteId: The .NET 'System.Int64' value type
###Citrix.StoreFront.Model.Authentication.AuthenticationService
Parameter AuthenticationService: A .NET class representing the configuration of a StoreFront Authentication service
###System.Management.Automation.SwitchParameter
Parameter Anonymous: The .NET 'System.Management.Automation.SwitchParameter' value type
###System.String
Parameter FarmName: The .NET 'System.String' reference type
###Citrix.StoreFront.Model.Store.FarmType
Parameter FarmType: The .NET 'Citrix.StoreFront.Model.Store.FarmType' value type
###System.String[]
Parameter Servers: The .NET 'System.String' reference type
###System.Int32
Parameter Port: The .NET 'System.Int32' value type
###Citrix.StoreFront.Model.Store.TransportType
Parameter TransportType: The .NET 'Citrix.StoreFront.Model.Store.TransportType' value type
###System.Int32
Parameter SSLRelayPort: The .NET 'System.Int32' value type
###System.Boolean
Parameter LoadBalance: The .NET 'System.Boolean' value type
###System.Int32
Parameter AllFailedBypassDuration: The .NET 'System.Int32' value type
###System.Int32
Parameter BypassDuration: The .NET 'System.Int32' value type
###System.String
Parameter FriendlyName: The .NET 'System.String' reference type
###System.String[]
Parameter Zones: The .NET 'System.String' reference type
###System.String
Parameter ConnectionString: The .NET 'System.String' reference type
##Return Values
###StoreService
A .NET class representing the configuration of a StoreFront Store service
##Examples
###EXAMPLE 1 Create a new Store
```
```
REMARKS
Creates a new Store using an existing Authentication Service
