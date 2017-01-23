#Remove-STFStoreFarm
Remove Farm from a Store
##Syntax
```
Remove-STFStoreFarm [-FarmName] <String[]> [-StoreService] <StoreService> [<CommonParameters>]
```
##Detailed Description
Removes a XenDesktop\XenApp farm from a Store service.
##Related Commands
*[Add-STFStoreFarm](Add-STFStoreFarm)
*[Set-STFStoreFarm](Set-STFStoreFarm)
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.Store.Farm[]
Parameter Farm: A .NET class representing the configuration of a Farm in StoreFront Store service
###System.String[]
Parameter FarmName: The .NET 'System.String' reference type
###Citrix.StoreFront.Model.Store.StoreService
Parameter StoreService: A .NET class representing the configuration of a StoreFront Store service
##Return Values
##Examples
###EXAMPLE 1 Remove a Farm from the Store service
```
$farm = Get-STFStoreFarm -StoreService $storeService -FarmName XenDesktop75
Remove-STFStoreFarm $farm -StoreService $storeService
```
REMARKS
Remove the Farm XenDesktop75 from the Store service.

```
Remove-STFStoreFarm -FarmName XenDesktop75 -StoreService $storeService
```
REMARKS
Remove the Farm XenDesktop75 with the specified name from the Store service.
