#Set-STFStoreService
Configure the Store service
##Syntax
```
```
##Detailed Description
Configure high level options on the Store service.
##Related Commands
*[Get-STFStoreService](Get-STFStoreService)
*[Remove-STFStoreService](Remove-STFStoreService)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.Store.StoreService
Parameter StoreService: A .NET class representing the configuration of a StoreFront Store service
###System.Boolean
Parameter RDPOnly: The .NET 'System.Boolean' value type
###System.String
Parameter IcaTemplateName: The .NET 'System.String' reference type
###System.Boolean
Parameter IcaFileSigning: The .NET 'System.Boolean' value type
###System.String
Parameter IcaFileSigningCertificateThumbprint: The .NET 'System.String' reference type
###System.String
Parameter IcaFileSigningHashAlgorithm: The .NET 'System.String' reference type
###Citrix.StoreFront.Model.Authentication.AuthenticationService
Parameter AuthenticationService: A .NET class representing the configuration of a StoreFront Authentication service
###System.Boolean
Parameter KerberosDelegation: The .NET 'System.Boolean' value type
###System.Management.Automation.SwitchParameter
Parameter Force: The .NET 'System.Management.Automation.SwitchParameter' value type
###System.Boolean
Parameter AllowSessionReconnect: The .NET 'System.Boolean' value type
###System.Boolean
Parameter SubstituteDesktopImage: The .NET 'System.Boolean' value type
###Citrix.StoreFront.Model.ReceiverForWeb.WebReceiverService
Parameter UnifiedReceiver: A .NET class representing the configuration of a StoreFront Web Receiver service
###System.Boolean
Parameter LockedDown: The .NET 'System.Boolean' value type
###System.Management.Automation.SwitchParameter
Parameter PassThru: The .NET 'System.Management.Automation.SwitchParameter' value type
##Return Values
##Examples
###EXAMPLE 1 Sign Ica files
```
Set-STFStoreService $storeService -IcaFileSigning $true -IcaFileSigningCertificateThumbprint a909502dd82ae41433e6f83886b00d4277a32a7b
```
REMARKS
Configure the Store to sign ica files using the certificate with the supplied
thumbprint.
