#Add-STFWebReceiverFeature
Add a feature to the WebReceiver service
##Syntax
```
Add-STFWebReceiverFeature [-FeatureClassId] <Guid> [-WebReceiverService] <WebReceiverService> [<CommonParameters>]
```
##Detailed Description
Adds a single feature to to the specified WebReceiver service.
##Related Commands
##Parameters
|Name|Description|Required?|Pipeline Input|
###System.String
Parameter Name: The .NET 'System.String' reference type
###System.Guid
Parameter FeatureClassId: The .NET 'System.Guid' value type
###Citrix.StoreFront.Model.ReceiverForWeb.WebReceiverService
Parameter WebReceiverService: A .NET class representing the configuration of a StoreFront Web Receiver service
##Return Values
##Examples
###EXAMPLE 1 Add an WebReceiver feature
```
Add-STFWebReceiverFeature -Name CustomSDK -WebReceiverService $rfw
```
REMARKS
Add the feature "CustomSDK" to the WebReceiver service /Citrix/StoreWeb
