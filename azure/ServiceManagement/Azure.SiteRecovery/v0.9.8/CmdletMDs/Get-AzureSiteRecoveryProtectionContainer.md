---
external help file: Microsoft.Azure.Commands.RecoveryServices.dll-Help.xml
online version: 41fb380e-9434-467a-84d4-1e0bcfe70590
schema: 2.0.0
updated_at: 10/14/2016 7:06 AM
ms.date: 10/14/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.SiteRecovery/v0.9.8/CmdletMDs/Get-AzureSiteRecoveryProtectionContainer.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/a56d0e01e65c2c33aa2af13dd29addc94ead6e88/azureps-cmdlets-docs/ServiceManagement/Azure.SiteRecovery/v0.9.8/CmdletMDs/Get-AzureSiteRecoveryProtectionContainer.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: Visual Studio China
keywords: powershell, content
manager: Visual Studio China
---

# Get-AzureSiteRecoveryProtectionContainer

## SYNOPSIS
Gets protected containers for a vault.

## SYNTAX

### Default (Default)
```
Get-AzureSiteRecoveryProtectionContainer [-Profile <AzureProfile>] [<CommonParameters>]
```

### ById
```
Get-AzureSiteRecoveryProtectionContainer -Id <String> [-Profile <AzureProfile>] [<CommonParameters>]
```

### ByName
```
Get-AzureSiteRecoveryProtectionContainer -Name <String> [-Profile <AzureProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureSiteRecoveryProtectionContainer** cmdlet gets protected containers for the current Microsoft Azure Site Recovery vault.
A protected container is a logical container for protected objects such as virtual machines.
Azure Site Recovery configures replication settings for protected containers.

## EXAMPLES

### Example 1: Get protected containers
```
PS C:\>Get-AzureSiteRecoveryProtectionContainer
Name                        : PrimaryCloud
ID                          : fd00d920-79e4-4f2d-a282-a779c0cecb7f_ce995917-c962-45d0-b7f3-9f408a4e1429
FabricObjectId              : fd00d920-79e4-4f2d-a282-a779c0cecb7f
FabricType                  : VMM
Type                        : VMM
ServerId                    : fd00d920-79e4-4f2d-a282-a779c0cecb7f
Role                        : Primary
AvailableProtectionProfiles : {ab01dcbe-9da0-4c31-9564-d6904cfadfde, ad388147-83de-4d2f-a09d-fa46c626747e}
```

This command gets the protected containers for the current vault.

## PARAMETERS

### -Id
Specifies the ID of a protected container to get.

```yaml
Type: String
Parameter Sets: ById
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the name of a protected container to get.

```yaml
Type: String
Parameter Sets: ByName
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Profile
Specifies an Azure profile.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS
