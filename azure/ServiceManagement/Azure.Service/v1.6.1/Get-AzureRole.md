---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: .\Set-AzureRole.md
schema: 2.0.0
ms.assetid: CA7F8777-4356-4FF2-8CA4-C1CB43CAEBA7
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v1.6.1/Get-AzureRole.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v1.6.1/Get-AzureRole.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureRole

## SYNOPSIS
Returns a list of roles in your Microsoft azure_2 service.

## SYNTAX

```
Get-AzureRole [-ServiceName] <String> [[-Slot] <String>] [[-RoleName] <String>] [-InstanceDetails]
 [-Profile <AzureSMProfile>] [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRole** cmdlet returns a list object with details on the roles in your Microsoft azure_2 service.
If you specify the *RoleName* parameter, **Get-AzureRole** returns details on that role only.
If you specify the *InstanceDetails* parameter, additional, instance-specific details are returned.

## EXAMPLES

### Example 1: Get a list of roles for a service
```
PS C:\>Get-AzureRole -ServiceName "MySvc01" -Slot "Production"
```

This command returns an object with details on all the production roles running on the MySvc01 service.

### Example 2: Get details on a role running on a service
```
PS C:\>Get-AzureRole -ServiceName "MySvc1" -Slot "Staging" -RoleName "MyTestVM3"
```

This command returns an object with details on the MyTestVM3 role, running on the staging environment of the MySvc01 service.

### Example 3: Get instance information on instances of a role running on a service
```
PS C:\>Get-AzureRole -ServiceName "MySvc01" -Slot "Production" -RoleName "MyTestVM02" -InstanceDetails
```

This command returns an object with details on the instances of the MyTestVM02 role running in the production environment on the MySvc01 service.

### Example 4: Get a table of the role instances associated with a service
```
PS C:\>Get-AzureRole -ServiceName "MySvc01" -Slot "Production" -InstanceDetails | Format-Table -Auto "InstanceName", "InstanceSize", "InstanceStatus"
```

This command returns a table of the instance name, size, and status of all role instances running in the production environment on the MySvc01 service.

## PARAMETERS

### -ServiceName
Specifies the name of the azure_2 service.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Slot
Specifies the azure_2 deployment environment.
psdx_paramvalues Production or Staging.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -RoleName
Specifies the name of the role to get.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -InstanceDetails
Specifies that this cmdlet returns details about the instances on each role.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Profile
ps_azureprofile_description

```yaml
Type: AzureSMProfile
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationAction
@{Text=}

```yaml
Type: ActionPreference
Parameter Sets: (All)
Aliases: infa

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InformationVariable
@{Text=}

```yaml
Type: String
Parameter Sets: (All)
Aliases: iv

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Set-AzureRole](./Set-AzureRole.md)


