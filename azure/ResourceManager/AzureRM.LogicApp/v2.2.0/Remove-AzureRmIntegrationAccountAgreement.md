---
external help file: Microsoft.Azure.Commands.LogicApp.dll-Help.xml
online version: 3239a014-7f3b-48e0-b5f3-ab9267892888
schema: 2.0.0
ms.assetid: B531615B-228F-4C28-859B-6D0D4F86894B
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.LogicApp/v2.2.0/Remove-AzureRmIntegrationAccountAgreement.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.LogicApp/v2.2.0/Remove-AzureRmIntegrationAccountAgreement.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Remove-AzureRmIntegrationAccountAgreement

## SYNOPSIS
Removes an integration account agreement.

## SYNTAX

```
Remove-AzureRmIntegrationAccountAgreement -ResourceGroupName <String> -Name <String> -AgreementName <String>
 [-Force] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmIntegrationAccountAgreement** cmdlet removes an integration account agreement from an Azure resource group.
Specify the integration account name, resource group name, and agreement name.

This module supports dynamic parameters.
To use a dynamic parameter, type it in the command.
To discover the names of dynamic parameters, type a hyphen (-) after the cmdlet name, and then press the Tab key repeatedly to cycle through the available parameters.
If you omit a required template parameter, the cmdlet prompts you for the value.

## EXAMPLES

### Example 1: Remove an integration account agreement by name
```
PS C:\>Remove-AzureRmIntegrationAccountAgreement -ResourceGroupName "ResourceGroup11" -Name "IntegrationAccount31" -AgreementName "IntegrationAccountAgreement06" -Force
```

This command removes the integration account agreement named IntegrationAccountAgreement06.
The command does not prompt you for confirmation.

## PARAMETERS

### -ResourceGroupName
Specifies the name of a resource group.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name of an integration account.

```yaml
Type: String
Parameter Sets: (All)
Aliases: ResourceName

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AgreementName
Specifies the name of the integration account agreement.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Forces the command to run without asking for user confirmation.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmIntegrationAccountAgreement](./Get-AzureRmIntegrationAccountAgreement.md)

[New-AzureRmIntegrationAccountAgreement](./New-AzureRmIntegrationAccountAgreement.md)

[Set-AzureRmIntegrationAccountAgreement](./Set-AzureRmIntegrationAccountAgreement.md)


