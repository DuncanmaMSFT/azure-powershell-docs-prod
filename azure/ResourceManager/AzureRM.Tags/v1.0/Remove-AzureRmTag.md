---
external help file: Microsoft.Azure.Commands.Tags.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=404174
schema: 2.0.0
ms.assetid: AC99BEDE-9BB0-4449-9947-6DBBB236758D
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Tags/v1.0/Remove-AzureRmTag.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Tags/v1.0/Remove-AzureRmTag.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Remove-AzureRmTag

## SYNOPSIS
Deletes predefined azure_2 tags or values.

## SYNTAX

```
Remove-AzureRmTag [-Name] <String> [[-Value] <String[]>] [-Force] [-PassThru] [-WhatIf] [-Confirm]
 [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureRmTag** cmdlet deletes predefined azure_2 tags and values from your subscription.
To delete particular values from a predefined tag, use the *Value* parameter.
By default, **Remove-AzureRmTag** deletes the specified tag and all of its values.You cannot delete a tag or value that is currently applied to a resource or resource group.

Before using **Remove-AzureRmTag**, use the *Tag* parameter of the Set-AzureRMResourceGroup cmdlet to delete the tag or values from the resource or resource group.

The azure_2 Tags module that **Remove-AzureRmTag** is part of can help you manage your predefined azure_2 tags.
An azure_2 tag is a name-value pair that you can use to categorize your azure_2 resources and resource groups, such as by department or cost center, or to track notes or comments about the resources and groups.

You can define and apply tags in a single step, but predefined tags let you establish standard, consistent, predictable names and values for the tags in your subscription.
If the subscription includes any predefined tags, you cannot apply undefined tags or values to any resource or resource group in the subscription.

## EXAMPLES

### Example 1: Delete a predefined tag
```
PS C:\>Remove-AzureRmTag -Name "Department"
```

This command deletes the predefined tag named Department and all of its resources.
If the tag has been applied to any resources or resource groups, the command fails.

### Example 2: Delete a value from a predefined tag
```
PS C:\>Remove-AzureRmTag -Name "Department" -Value "HumanResources" -PassThru
Name:   Department
Count:  14
Values: 

        Name        Count
        =========   =====

        Finance        2
        IT            12
```

This command deletes the HumanResources value from the predefined Department tag.
It does not delete the tag.
If the value has been applied to any resources or resource groups, the command fails.

## PARAMETERS

### -Force
Forces the command to run without asking for user confirmation.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Name
Specifies the name of the tag to be deleted.
By default, **Remove-AzureRmTag** removes the specified tag and all of its values.
To delete selected values, but not delete the tag, use the *Value* parameter.

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

### -PassThru
Returns an object that represents the deleted tag or the resulting tag with deleted valued.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Value
Deletes the specified values from the predefined tag, but does not delete the tag.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Confirm
psdx_confirmdesc

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

### -WhatIf
psdx_whatifdesc

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None

## OUTPUTS

### None or Microsoft.Azure.Commands.Tags.Model.PSTag

## NOTES

## RELATED LINKS

[Get-AzureRmTag](./Get-AzureRmTag.md)

[New-AzureRmTag](./New-AzureRmTag.md)


