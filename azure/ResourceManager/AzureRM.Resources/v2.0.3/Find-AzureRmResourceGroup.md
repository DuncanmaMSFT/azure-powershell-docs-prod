---
external help file: Microsoft.Azure.Commands.ResourceManager.Cmdlets.dll-Help.xml
online version: 7827edc2-87d5-4885-b853-cb48b5847a16
schema: 2.0.0
ms.assetid: 7827EDC2-87D5-4885-B853-CB48B5847A16
updated_at: 10/18/2016 9:38 PM
ms.date: 10/18/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v2.0.3/Find-AzureRmResourceGroup.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/23cdb8705d4ab9807c0e21b238f3b134a7d49c7d/azureps-cmdlets-docs/ResourceManager/AzureRM.Resources/v2.0.3/Find-AzureRmResourceGroup.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
---

# Find-AzureRmResourceGroup

## SYNOPSIS
Searches for resource groups.

## SYNTAX

```
Find-AzureRmResourceGroup [-Tag <Hashtable>] [-ApiVersion <String>] [-Pre] [<CommonParameters>]
```

## DESCRIPTION
The **Find-AzureRmResourceGroup** cmdlet searches for resource groups using the specified parameters.

## EXAMPLES

### Example 1: Find all resource groups
```
PS C:\>Find-AzureRmResourceGroup
```

This command finds all resource groups.

### Example 2: Find resource groups by tag name
```
PS C:\>Find-AzureRmResourceGroup -Tag @{ Name = "testtag" }
```

This command finds all resource groups that have a tag named testtag.

### Example 3: Find resource groups by tag name and value
```
PS C:\>Find-AzureRmResourceGroup -Tag @{ Name = "testtag"; Value = "testval" }
```

This command finds all resource groups that have a tag named testtag and the value testval.

## PARAMETERS

### -Tag
Specifies tag information, as a hash table, to filter your results.
Use the following formats: 

`@{Name = '`tagName`'}`
`@{Name = '`tagName`'; Value = '`tagValue`'}`

```yaml
Type: Hashtable
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ApiVersion
Specifies the version of the resource provider API to use.
If you do not specify a version, this cmdlet uses the latest available version.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Pre
Indicates that this cmdlet considers pre-release API versions when it automatically determines which version to use.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS


