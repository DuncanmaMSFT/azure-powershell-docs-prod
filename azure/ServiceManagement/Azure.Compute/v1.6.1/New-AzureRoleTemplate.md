---
external help file: Microsoft.WindowsAzure.Commands.dll-Help.xml
online version: 
schema: 2.0.0
ms.assetid: 03FBB075-4258-4EB3-A5D1-3AE0F599E361
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v1.6.1/New-AzureRoleTemplate.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.Compute/v1.6.1/New-AzureRoleTemplate.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# New-AzureRoleTemplate

## SYNOPSIS
Creates web and worker role templates.

## SYNTAX

### WebRole
```
New-AzureRoleTemplate [-Web] [[-Output] <String>] [-Profile <AzureSMProfile>] [<CommonParameters>]
```

### WorkerRole
```
New-AzureRoleTemplate [-Worker] [[-Output] <String>] [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
powershell_prelim

The **New-AzureRoleTemplate** cmdlet creates web and worker role templates.

## EXAMPLES

### 1: Create a web role template
```
PS C:\>New-AzureRoleTemplate -Web
```

This example creates a new web role template in a folder named WebRoleTemplate in the current directory.

### 2: Create a worker role template
```
PS C:\>New-AzureRoleTemplate -Worker
```

This example creates a new worker role template in a folder named WebRoleTemplate in the current directory.

### 3: Create a role template in a custom directory
```
PS C:\>New-AzureRoleTemplate -Web -Output C:\MyWebRoleTemplate
```

This example creates a new web role template in directory named MyWebRoleTemplate, instead of in the current directory.

## PARAMETERS

### -Web
Specifies that you want to create a web role template.

```yaml
Type: SwitchParameter
Parameter Sets: WebRole
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Worker
Specifies that you want to create a worker role template.

```yaml
Type: SwitchParameter
Parameter Sets: WorkerRole
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Output
Specifies the output path of generated template.
\<Unclear to me ¢â‚¬Â¦is this where you want to store the template that the cmdlet creates?
Seems to be based on the example.\>

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

[Add-AzureWebRole](./Add-AzureWebRole.md)

[Add-AzureWorkerRole](./Add-AzureWorkerRole.md)


