---
external help file: Microsoft.WindowsAzure.Commands.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 775B1B1E-464E-4464-B134-747D53913F49
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v2.1.0/New-AzureServiceProject.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v2.1.0/New-AzureServiceProject.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# New-AzureServiceProject

## SYNOPSIS
Creates the required files and configuration (sometimes referred to as scaffolding) for a new service.

## SYNTAX

```
New-AzureServiceProject [-ServiceName] <String> [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
This topic describes the cmdlet in the 0.8.10 version of the Microsoft Azure PowerShell module.
To get the version of the module you're using, in the Azure PowerShell console, type (Get-Module -Name Azure).Version.

The **New-AzureServiceProject** cmdlet creates the required files and configuration for a new Azure service in the current directory.

## EXAMPLES

### 1:
```
PS C:\>New-AzureServiceProject MyService1
```

This example creates scaffolding for a new Azure service named  ¢â‚¬Å"MyService1 ¢â‚¬Â in the current directory.

## PARAMETERS

### -ServiceName
Specifies the name of the service.
It determines the first section of the hostname for your service (for example, name.cloudapp.net), and the directory that will contain your service.
The name can contain only letters, digits, and the dash character (-).

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

### -Profile
In-memory profile.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Add-AzureNodeWebRole](./Add-AzureNodeWebRole.md)

[Add-AzureNodeWorkerRole](./Add-AzureNodeWorkerRole.md)

[Set-AzureServiceProject](./Set-AzureServiceProject.md)

[Set-AzureServiceProjectRole](./Set-AzureServiceProjectRole.md)


