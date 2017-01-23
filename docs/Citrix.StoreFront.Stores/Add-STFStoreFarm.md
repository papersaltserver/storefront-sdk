#Add-STFStoreFarm
Add a farm to a Store
##Syntax
```
Add-STFStoreFarm [-FarmName] <String> [-FarmType] <XenApp | XenDesktop | AppController | VDIinaBox> [-Servers] <String[]> [[-Port] <Int32>] [[-TransportType] <HTTP | HTTPS | SSL>] [[-SSLRelayPort] <Int32>] [[-LoadBalance] <Boolean>] [[-AllFailedBypassDuration] <Int32>] [[-BypassDuration] <Int32>] [[-TicketTimeToLive] <Int32>] [[-RadeTicketTimeToLive] <Int32>] [[-MaxFailedServersPerRequest] <Int32>] [[-Zones] <String[]>] [[-PassThru] <SwitchParameter>] [-StoreService] <StoreService> [<CommonParameters>]
```
##Detailed Description
Add a XenApp \ XenDesktop farm to the specified Store service.
##Related Commands
*[Remove-STFStoreFarm](Remove-STFStoreFarm)
*[Get-STFStoreFarm](Get-STFStoreFarm)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.Store.Farm
Parameter Farm: A .NET class representing the configuration of a Farm in StoreFront Store service
###Citrix.StoreFront.Model.Store.StoreService
Parameter StoreService: A .NET class representing the configuration of a StoreFront Store service
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
###System.Int32
Parameter TicketTimeToLive: The .NET 'System.Int32' value type
###System.Int32
Parameter RadeTicketTimeToLive: The .NET 'System.Int32' value type
###System.Int32
Parameter MaxFailedServersPerRequest: The .NET 'System.Int32' value type
###System.String[]
Parameter Zones: The .NET 'System.String' reference type
###System.Management.Automation.SwitchParameter
Parameter PassThru: The .NET 'System.Management.Automation.SwitchParameter' value type
##Return Values
###Farm
A .NET class representing the configuration of a Farm in StoreFront Store service
##Examples
###EXAMPLE 1 Copy a farm from the Store service at /Citrix/Store1 to the Store service at /Citrix/Store2
```
$farm = $store1.FarmsConfiguration.Farms[0]
$store2 = Get-STFStoreService -VirtualPath /Citrix/Store2
Add-STFStoreFarm -StoreService $store2 -Farm $farm
```
REMARKS
Adds a new farm to $store2 with the same properties as the first farm from
$store1. The farm object ($farm) is not changed by this operation.

```
Add-STFStoreFarm -StoreService $store -FarmName "XenDesktop75" -FarmType XenDesktop -Port 80 -TransportType HTTP -Servers Xen1
```
REMARKS
Adds the Xen1 XenDesktop server to the XenDesktop75 farm

```
Add-STFStoreFarm -StoreService $store -FarmName "XenDesktop75" -FarmType XenDesktop -Port 80 -TransportType HTTP -Servers Xen1
```
REMARKS
Adds the Xen1 XenDesktop server to the XenDesktop75 farm
