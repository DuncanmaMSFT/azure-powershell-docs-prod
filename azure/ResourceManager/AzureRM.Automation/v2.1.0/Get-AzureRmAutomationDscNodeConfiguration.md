---
external help file: Microsoft.Azure.Commands.ResourceManager.Automation.dll-Help.xml
online version: .\Import-AzureRmAutomationDscNodeConfiguration.md
schema: 2.0.0
ms.assetid: 16207DEE-029F-4659-AB6F-F636F869B82B
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Automation/v2.1.0/Get-AzureRmAutomationDscNodeConfiguration.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Automation/v2.1.0/Get-AzureRmAutomationDscNodeConfiguration.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
---

# Get-AzureRmAutomationDscNodeConfiguration

## SYNOPSIS
Gets metadata for DSC node configurations in Automation.

## SYNTAX

### ByAll (Default)
```
Get-AzureRmAutomationDscNodeConfiguration [-RollupStatus <String>] [-ResourceGroupName] <String>
 [-AutomationAccountName] <String> [<CommonParameters>]
```

### ByNodeConfigurationName
```
Get-AzureRmAutomationDscNodeConfiguration -Name <String> [-ResourceGroupName] <String>
 [-AutomationAccountName] <String> [<CommonParameters>]
```

### ByConfigurationName
```
Get-AzureRmAutomationDscNodeConfiguration -ConfigurationName <String> [-RollupStatus <String>]
 [-ResourceGroupName] <String> [-AutomationAccountName] <String> [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmAutomationDscNodeConfiguration** cmdlet gets metadata for Azure PowerShell Desired State Configuration (DSC) node configurations in Azure Automation.
Automation stores DSC node configuration as a Managed Object Format (MOF) configuration document.

## EXAMPLES

### Example 1: Get all DSC node configurations
```
PS C:\>Get-AzureRmAutomationDscNodeConfiguration -ResourceGroupName "ResourceGroup03" -AutomationAccountName "Contoso17"
```

This command gets metadata for all DSC node configurations in the Automation account named Contoso17.

### Example 2: Get all DSC node configurations for a DSC configuration
```
PS C:\>Get-AzureRmAutomationDscNodeConfiguration -ResourceGroupName "ResourceGroup03" -AutomationAccountName "Contoso17" -ConfigurationName "ContosoConfiguration"
```

This command gets metadata for all DSC node configurations in the Automation account named Contoso17 that the DSC configuration named ContosoConfiguration generated.

### Example 3: Get a DSC node configuration by name
```
PS C:\>Get-AzureRmAutomationDscNodeConfiguration -ResourceGroupName "ResourceGroup03" -AutomationAccountName "Contoso17" -Name "ContosoConfiguration.webserver"
```

This command gets metadata for a DSC node configuration with the name ContosoConfiguration.webserver in the Automation account named Contoso17.

## PARAMETERS

### -AutomationAccountName
Specifies the name of an Automation account that contains the DSC node configurations for which this cmdlet gets metadata.

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

### -ConfigurationName
Specifies the name of DSC configuration for which this cmdlet gets node configuration metadata.

```yaml
Type: String
Parameter Sets: ByConfigurationName
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name of the DSC node configuration for which this cmdlet gets metadata.

```yaml
Type: String
Parameter Sets: ByNodeConfigurationName
Aliases: NodeConfigurationName

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of a resource group.
This cmdlet gets metadata for DSC node configurations in the resource group that this parameter specifies.

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

### -RollupStatus
Specifies the rollup status of DSC node configurations that this cmdlet gets.
Valid values are: 

- Bad 
- Good

```yaml
Type: String
Parameter Sets: ByAll, ByConfigurationName
Aliases: 
Accepted values: Good, Bad

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

[Import-AzureRmAutomationDscNodeConfiguration](./Import-AzureRmAutomationDscNodeConfiguration.md)


