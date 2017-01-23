#Clear-STFWebReceiverClientPlugin
Clears the plug-ins definitions configured within the WebReceiver
##Syntax
```
```
##Detailed Description
The cmdlet clears the plug-ins definitions as configured within the WebReceiver.
##Related Commands
*[Add-STFWebReceiverClientPlugin](Add-STFWebReceiverClientPlugin)
*[Remove-STFWebReceiverClientPlugin](Remove-STFWebReceiverClientPlugin)
*[Set-STFWebReceiverClientPlugin](Set-STFWebReceiverClientPlugin)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.ReceiverForWeb.WebReceiverService
Parameter WebReceiverService: A .NET class representing the configuration of a StoreFront Web Receiver service
##Return Values
##Examples
###EXAMPLE 1 Clear client plugins
```
Clear-STFWebReceiverClientPlugins -WebReceiverService $webReceiver
```
REMARKS
Clear all plug-ins from the only configured WebReceiver service.
