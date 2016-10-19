---
external help file: Microsoft.Azure.Commands.Compute.dll-Help.xml
online version: .\Add-AzureRmContainerServiceAgentPoolProfile.md
schema: 2.0.0
ms.assetid: C52E74C1-9D28-4253-86D3-91AD50902A11
updated_at: 10/18/2016 9:38 PM
ms.date: 10/18/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.1.0/Remove-AzureRmContainerServiceAgentPoolProfile.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/23cdb8705d4ab9807c0e21b238f3b134a7d49c7d/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.1.0/Remove-AzureRmContainerServiceAgentPoolProfile.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Remove-AzureRmContainerServiceAgentPoolProfile

## SYNOPSIS
Removes an agent pool profile from a container service.

## SYNTAX

```
Remove-AzureRmContainerServiceAgentPoolProfile [-ContainerService] <ContainerService> [-Name] <String>
 [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmContainerServiceAgentPoolProfile** cmdlet removes an agent pool profile from a container service.

## EXAMPLES

### Example 1: Remove a profile from a container service
```
PS C:\>$Container = Get-AzureRmContainerService -ResourceGroupName "ResourceGroup17" -Name "CSResourceGroup17" 
PS C:\> Remove-AzureRmContainerServiceAgentPoolProfile -ContainerService $Container -Name "AgentPool01"
```

The first command gets a container service named CSResourceGroup17 by using the Get-AzureRmContainerService cmdlet.
The command stores the service in the $Container variable.

The second command removes the profile named AgentPool01 from the container service in $Container.

## PARAMETERS

### -ContainerService
Specifies the container service object from which this cmdlet removes an agent pool profile.

```yaml
Type: ContainerService
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -Name
Specifies the name of the agent pool profile that this cmdlet removes.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Add-AzureRmContainerServiceAgentPoolProfile](.\Add-AzureRmContainerServiceAgentPoolProfile.md)

[Get-AzureRmContainerService](.\Get-AzureRmContainerService.md)

