#Get-STFWebReceiverDiscoveryService
Get the WebReceiver Discovery Service settings
##Syntax
```
```
##Detailed Description
Get the WebReceiver Discovery Service settings.
##Related Commands
*[Set-STFWebReceiverDiscoveryService](Set-STFWebReceiverDiscoveryService)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.ReceiverForWeb.WebReceiverService
Parameter WebReceiverService: A .NET class representing the configuration of a StoreFront Web Receiver service
##Return Values
###DiscoveryService
The .NET 'Citrix.StoreFront.Model.ReceiverForWeb.DiscoveryService' reference type
##Examples
###EXAMPLE 1 Get Discovery Service settings
```
Get-STFWebReceiverDiscoveryService $webReceiver
```
REMARKS
Get the WebReceiver Discovery Service settings for /Citrix/StoreWeb.
OUTPUT
```
RunDiscoveryAtStart : True
```