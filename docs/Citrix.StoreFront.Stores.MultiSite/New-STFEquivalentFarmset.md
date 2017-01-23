#New-STFEquivalentFarmset
Create a new EquivalentFarmSet for a UserFarmMapping.
##Syntax
```
```
##Detailed Description
An EquivalentFarmSet is a set of PrimaryFarms that are considered to be identical. The applications and desktops available are equivalent so the experience of using any of the PrimaryFarms would be identical to an end user.If a farm is not identical then the applications and desktops available during enumeration and launch may vary as requests are load balanced or failed over between farms. If this is the case consider creating a second EquivalentFarmSet and give them both the same AggregationGroupName to remove any duplicate (or overlapping) applications and desktops.EquivalentFarmSets also define BackupFarms, they will only be used should all PrimaryFarms and EquivalentFarmsSets with identical AggregationGroupName become unavailable.
##Related Commands
*[New-STFEquivalentFarmset](New-STFEquivalentFarmset)
*[Get-STFUserFarmMapping](Get-STFUserFarmMapping)
*[Clear-STFUserFarmMappings](Clear-STFUserFarmMappings)
*[New-STFUserFarmMappingGroup](New-STFUserFarmMappingGroup)
*[Set-STFUserFarmMapping](Set-STFUserFarmMapping)
##Parameters
|Name|Description|Required?|Pipeline Input|
###System.String
Parameter Name: The .NET 'System.String' reference type
###System.String
Parameter AggregationGroupName: The .NET 'System.String' reference type
###System.String[]
Parameter PrimaryFarms: The .NET 'System.String' reference type
###System.String[]
Parameter BackupFarms: The .NET 'System.String' reference type
###Citrix.StoreFront.Model.Store.LoadBalanceMode
Parameter LoadBalanceMode: The .NET 'Citrix.StoreFront.Model.Store.LoadBalanceMode' value type
##Return Values
###EquivalentFarmSet
The .NET 'Citrix.StoreFront.Model.Store.EquivalentFarmSet' reference type
##Notes
Must be added to a UserFarmMapping via the Set-STFUserFarmMapping cmdlet before it can be used.
##Examples
###EXAMPLE 1 Create a new EquivalentFarmSet
```
```
REMARKS
Creates a new EquivalentFarmSet with two servers XenApp1 and XenApp2 that will
be load balanced. Should the primary server fail XenAppBackup will be used.
