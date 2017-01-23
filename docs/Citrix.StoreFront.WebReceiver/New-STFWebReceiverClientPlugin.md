#New-STFWebReceiverClientPlugin
Create a WebReceiver client plug-in
##Syntax
```
```
##Detailed Description
Create WebReceiver script and branding customizations.
##Related Commands
*[Add-STFWebReceiverClientPlugin](Add-STFWebReceiverClientPlugin)
*[Set-STFWebReceiverClientPlugin](Set-STFWebReceiverClientPlugin)
*[Clear-STFWebReceiverClientPlugin](Clear-STFWebReceiverClientPlugin)
*[Remove-STFWebReceiverClientPlugin](Remove-STFWebReceiverClientPlugin)
##Parameters
|Name|Description|Required?|Pipeline Input|
###System.String
Parameter Name: The .NET 'System.String' reference type
###System.String
Parameter Source: The .NET 'System.String' reference type
###System.String[]
Parameter Scripts: The .NET 'System.String' reference type
###System.String[]
Parameter Styles: The .NET 'System.String' reference type
###System.Collections.Hashtable
Parameter Parameters: The .NET 'System.Collections.Hashtable' reference type
##Return Values
###ClientPlugin
The .NET 'Citrix.StoreFront.Model.ReceiverForWeb.ClientPlugin' reference type
##Examples
###EXAMPLE 1 Create a new client plugin
```
- Source "/plugins/netscalar/script1.js" `
-Scripts @("/ plugins/netscalar/script2.js", "/ plugins/netscalar/script1.js") `
-Styles @("/ plugins/netscalar/script2.css", "/ plugins/netscalar/script1.css") `
-Parameters @{"param1" = "value1";"param2" = "value2"}
```
REMARKS
Creates a new client plug-in for assignment to a WebReceiver.
