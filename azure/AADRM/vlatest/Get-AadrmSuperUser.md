---
external help file: Microsoft.RightsManagementServices.Online.Admin.PowerShell.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=400614
schema: 2.0.0
ms.assetid: 508FBF5B-A405-4FCB-9EB3-39183F46F60A
updated_at: 10/18/2016 11:27 PM
ms.date: 10/18/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/aip-cmdlets/AADRM/vlatest/Get-AadrmSuperUser.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/3cd0578639ed506752c7be4e6fb9013725a24d6f/aip-cmdlets/AADRM/vlatest/Get-AadrmSuperUser.md
ms.topic: reference
ms.prod: powershell
ms.service: rights-management
ms.technology: Azure Powershell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AadrmSuperUser

## SYNOPSIS
Gets the super users for Rights Management.

## SYNTAX

```
Get-AadrmSuperUser [<CommonParameters>]
```

## DESCRIPTION
The **Get-AadrmSuperUser** cmdlet gets the super users for Azure Rights Management, who can unprotect or protect files for your organization when the super user feature is enabled by using the Enable-AadrmSuperUserFeature cmdlet.
For more information about super users, see Configuring super users for Azure Rights Management and discovery services or data recoveryhttps://docs.microsoft.com/rights-management/deploy-use/configure-super-users (https://docs.microsoft.com/rights-management/deploy-use/configure-super-users) on the Microsoft documentation site.

## EXAMPLES

### Example 1: List super users
```
PS C:\>Get-AadrmSuperUser
```

This command lists the super users for Rights Management.

## PARAMETERS

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Add-AadrmSuperUser](.\Add-AadrmSuperUser.md)

[Remove-AadrmSuperUser](.\Remove-AadrmSuperUser.md)

[Enable-AadrmSuperUserFeature](.\Enable-AadrmSuperUserFeature.md)


