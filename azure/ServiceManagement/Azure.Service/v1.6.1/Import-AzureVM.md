---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: .\Export-AzureVM.md
schema: 2.0.0
ms.assetid: 349D54F9-A5F7-460E-B5C8-FDAADC5EB4C7
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v1.6.1/Import-AzureVM.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v1.6.1/Import-AzureVM.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Import-AzureVM

## SYNOPSIS
Imports an azure_2 virtual machine state from a file.

## SYNTAX

```
Import-AzureVM [-Path] <String> [-InformationAction <ActionPreference>] [-InformationVariable <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Import-AzureVM** cmdlet imports the previously saved state of a virtual machine from an XML file.
This cmdlet is useful when you want to subsequently create a virtual machine from the imported data.

Running **Export-AzureVM**, followed by **Remove-AzureVM** and then **Import-AzureVM** to recreate a virtual machine can cause the resultant virtual machine to have a different IP address than the original.

## EXAMPLES

### Example 1: Import a virtual machine state
```
PS C:\>Import-AzureVM -Path "C:\VMstate.xml" | New-AzureVM -ServiceName "ContosoService02"
```

This command imports the state of a virtual machine from the VMstate.xml file, and then creates a virtual machine in the specified cloud service.

## PARAMETERS

### -Path
Specifies the path of the file with the previously saved virtual machine state.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
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

[Export-AzureVM](./Export-AzureVM.md)

[New-AzureVM](./New-AzureVM.md)


