---
external help file: Microsoft.WindowsAzure.Commands.RemoteApp.dll-Help.xml
online version: .\Get-AzureRemoteAppWorkspace.md
schema: 2.0.0
updated_at: 10/14/2016 7:06 AM
ms.date: 10/14/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.RemoteApp/v1.0/CmdletMDs/Set-AzureRemoteAppWorkspace.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/a56d0e01e65c2c33aa2af13dd29addc94ead6e88/azureps-cmdlets-docs/ServiceManagement/Azure.RemoteApp/v1.0/CmdletMDs/Set-AzureRemoteAppWorkspace.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: Visual Studio China
keywords: powershell, content
manager: Visual Studio China
---

# Set-AzureRemoteAppWorkspace

## SYNOPSIS
Sets the properties of an azure_2 RemoteApp workspace.

## SYNTAX

```
Set-AzureRemoteAppWorkspace [-WorkspaceName] <String> [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Set-AzureRemoteAppWorkspace** cmdlet sets the properties of an azure_2 RemoteApp workspace.

## EXAMPLES

### Example 1: Set the workspace name
```
PS C:\>Set-AzureRemoteAppWorkspace -WorkspaceName "Contoso Work Applications"
TrackingId
----------
12345
```

This command sets the azure_2 RemoteApp workspace name to Contoso Work Applications.

## PARAMETERS

### -WorkspaceName
Specifies the name of the azure_2 RemoteApp workspace.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -Profile
ps_azureprofile_description

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
* All azure_2 RemoteApp collections for a specified subscription exist within a shared workspace.

## RELATED LINKS

[Get-AzureRemoteAppWorkspace](.\Get-AzureRemoteAppWorkspace.md)
