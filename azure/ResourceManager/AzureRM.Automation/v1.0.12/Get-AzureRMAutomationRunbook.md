---
external help file: Microsoft.Azure.Commands.ResourceManager.Automation.dll-Help.xml
online version: .\Export-AzureRMAutomationRunbook.md
schema: 2.0.0
ms.assetid: 71DA0434-5C0F-498F-91F2-F09117DFA7CA
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Automation/v1.0.12/Get-AzureRMAutomationRunbook.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Automation/v1.0.12/Get-AzureRMAutomationRunbook.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
---

# Get-AzureRmAutomationRunbook

## SYNOPSIS
Gets a runbook.

## SYNTAX

### ByAll (Default)
```
Get-AzureRmAutomationRunbook [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 [<CommonParameters>]
```

### ByRunbookName
```
Get-AzureRmAutomationRunbook [-Name] <String> [-ResourceGroupName] <String> [-AutomationAccountName] <String>
 [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRmAutomationRunbook** cmdlet gets azure_2 Automation runbooks.
To get a specific runbook, specify its name.

## EXAMPLES

### Example 1: Get all runbooks
```
PS C:\>Get-AzureRmAutomationRunbook -AutomationAccountName "Contoso17" -ResourceGroupName "ResourceGroup01"
```

This command gets all runbooks in the azure_2 Automation account named Contoso17.

## PARAMETERS

### -AutomationAccountName
Specifies the name of an Automation account in which this cmdlet gets runbooks.

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

### -Name
Specifies the name of a runbook that this cmdlet gets.

```yaml
Type: String
Parameter Sets: ByRunbookName
Aliases: RunbookName

Required: True
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceGroupName
Specifies the name of the resource group for which this cmdlet gets runbooks.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### Microsoft.Azure.Commands.Automation.Model.Runbook

## NOTES

## RELATED LINKS

[Export-AzureRmAutomationRunbook](./Export-AzureRMAutomationRunbook.md)

[Import-AzureRmAutomationRunbook](./Import-AzureRMAutomationRunbook.md)

[New-AzureRmAutomationRunbook](./New-AzureRMAutomationRunbook.md)

[New-AzureRmAutomationRunbook](./New-AzureRMAutomationRunbook.md)

[Publish-AzureRmAutomationRunbook](./Publish-AzureRMAutomationRunbook.md)

[Remove-AzureRmAutomationRunbook](./Remove-AzureRMAutomationRunbook.md)

[Set-AzureRmAutomationRunbook](./Set-AzureRMAutomationRunbook.md)

[Start-AzureRmAutomationRunbook](./Start-AzureRMAutomationRunbook.md)


