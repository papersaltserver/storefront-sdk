#Get-STFRoamingAccount
Get the Roaming account
##Syntax
```
```
##Detailed Description
Get the Roaming account details for one or all Stores.
##Related Commands
##Parameters
|Name|Description|Required?|Pipeline Input|
###Citrix.StoreFront.Model.Store.StoreService
Parameter StoreService: A .NET class representing the configuration of a StoreFront Store service
##Return Values
###Accounts
The .NET 'Citrix.StoreFront.Model.Roaming.Accounts' reference type
##Examples
###EXAMPLE 1 Get Roaming account for a specific Store
```
Get-STFRoamingAccount -StoreService $store
```
REMARKS
Get the Roaming account for the only configured Store service.
