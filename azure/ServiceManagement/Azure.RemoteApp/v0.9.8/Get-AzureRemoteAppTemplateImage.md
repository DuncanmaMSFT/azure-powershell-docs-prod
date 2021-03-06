---
external help file: Microsoft.WindowsAzure.Commands.RemoteApp.dll-Help.xml
online version: .\Get-AzureRemoteAppCollection.md
schema: 2.0.0
ms.assetid: 0DA1D4D0-600C-466E-A541-F6D3142B91F9
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.RemoteApp/v0.9.8/Get-AzureRemoteAppTemplateImage.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.RemoteApp/v0.9.8/Get-AzureRemoteAppTemplateImage.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AzureRemoteAppTemplateImage

## SYNOPSIS
Retrieves information about RemoteApp template images in Azure.

## SYNTAX

```
Get-AzureRemoteAppTemplateImage [[-ImageName] <String>] [-Profile <AzureProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AzureRemoteAppTemplateImage** cmdlet retrieves information about Azure RemoteApp template images in Microsoft Azure.
This cmdlet returns an object containing information about a specified template image.
If no template image is specified, it retrieves information about all the template images in the current subscription.

## EXAMPLES

### Example 1: Get a list of all template images
```
PS C:\>Get-AzureRemoteAppTemplateImage
```

This command returns the list of all template images.

### Example 2: Retrieve information about a specified template image
```
PS C:\>Get-AzureRemoteAppTemplateImage -ImageName "ContosoApps"
```

This command retrieves information about the template image named ContosoApps.

## PARAMETERS

### -ImageName
Specifies the name of a RemoteApp template image.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Profile
Specifies the Azure profile from which this cmdlet reads.
If you do not specify a profile, this cmdlet reads from the local default profile.

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

[Get-AzureRemoteAppCollection](./Get-AzureRemoteAppCollection.md)

[Get-AzureRemoteAppStartMenuProgram](./Get-AzureRemoteAppStartMenuProgram.md)


