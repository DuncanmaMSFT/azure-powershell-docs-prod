---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.Network.dll-Help.xml
online version: fd6f1d91-f019-4282-9f4f-46aeb4b4621b
schema: 2.0.0
ms.assetid: F2CBB48C-05F9-408F-9544-9DADCE1118DE
updated_at: 10/20/2016 12:12 AM
ms.date: 10/20/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v0.9.8/Get-AzureEffectiveRouteTable.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/831f900c1a4babea8fcc8817cfbc25252a1aa872/azureps-cmdlets-docs/ServiceManagement/Azure.Networking/v0.9.8/Get-AzureEffectiveRouteTable.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureEffectiveRouteTable

## SYNOPSIS
Gets the route applied in a virtual machine.

## SYNTAX

### IaaSGetEffectiveRouteTableParamSet
```
Get-AzureEffectiveRouteTable [-VM] <PersistentVMRoleContext> [-ServiceName] <String>
 [[-NetworkInterfaceName] <String>] [-Profile <AzureProfile>] [-PipelineVariable <String>] [<CommonParameters>]
```

### SlotGetEffectiveRouteTableParamSet
```
Get-AzureEffectiveRouteTable [-ServiceName] <String> [[-Slot] <String>] [-RoleInstanceName] <String>
 [[-NetworkInterfaceName] <String>] [-Profile <AzureProfile>] [-PipelineVariable <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureEffectiveRouteTable** cmdlet gets the route applied in a virtual machine.
This operation could take several seconds to finish.

## EXAMPLES

### Example 1: Get the route applied a virtual machine
```
PS C:\>Get-AzureVM -ServiceName "ContosoService" -Name "ContosoVM06" | Get-AzureEffectiveRouteTable
```

This command gets a virtual machine named ContosoVM06 for the service named ContosoService, and passes that virtual machine object to the current cmdlet.
The current cmdlet gets the route applied to that virtual machine.

## PARAMETERS

### -NetworkInterfaceName
Specifies the name of the network adapter for which this cmdlet gets effective routes.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 4
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -PipelineVariable
Not Specified

```yaml
Type: String
Parameter Sets: (All)
Aliases: pv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Profile
Specifies the Azure profile from which this cmdlet reads.
If you do not specify a profile, this cmdlet reads from the local default profile.

```yaml
Type: AzureProfile
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -RoleInstanceName
Specifies the name of a PaaS role for which this cmdlet gets effective routes.

```yaml
Type: String
Parameter Sets: SlotGetEffectiveRouteTableParamSet
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ServiceName
Specifies the name of a cloud service.
The PaaS role for which this cmdlet gets effective routes belongs to the service that this parameter specifies.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Slot
Specifies a PaaS slot.
The PaaS role for which this cmdlet gets effective routes has the slot that this parameter specifies.
Valid values are: 

- Production
- Staging 

The default value is Production.

```yaml
Type: String
Parameter Sets: SlotGetEffectiveRouteTableParamSet
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -VM
Specifies the virtual machine object for which this cmdlet gets effective routes.

```yaml
Type: PersistentVMRoleContext
Parameter Sets: IaaSGetEffectiveRouteTableParamSet
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### System.Collections.Generic.IEnumerable<Microsoft.WindowsAzure.Management.Network.Models.EffectiveRouteTable, Microsoft.WindowsAzure.Management.Network>

## NOTES

## RELATED LINKS


