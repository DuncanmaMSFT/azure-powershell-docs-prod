---
external help file: Microsoft.RightsManagementServices.Online.Admin.PowerShell.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=400619
schema: 2.0.0
ms.assetid: A3A194BD-D7B2-417F-902D-33D40BB3B332
updated_at: 10/18/2016 11:27 PM
ms.date: 10/18/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/aip-cmdlets/AADRM/vlatest/Get-AadrmUsageLogStorageAccount.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/3cd0578639ed506752c7be4e6fb9013725a24d6f/aip-cmdlets/AADRM/vlatest/Get-AadrmUsageLogStorageAccount.md
ms.topic: reference
ms.prod: powershell
ms.service: rights-management
ms.technology: Azure Powershell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Get-AadrmUsageLogStorageAccount

## SYNOPSIS
Gets the location for usage logs.

## SYNTAX

```
Get-AadrmUsageLogStorageAccount [<CommonParameters>]
```

## DESCRIPTION
The **Get-AadrmUsageLogStorageAccount** cmdlet gets the Azure storage location for usage logs for Azure Rights Management.

Note: This cmdlet should be used only if you have usage logs prior to the usage logging change in February 2016.
After this date, the only Windows PowerShell cmdlet that you need for Azure RMS usage logging is Get-AadrmUserLog.

For more information about usage logging, see Logging and analyzing Azure Rights Management usagehttps://docs.microsoft.com/rights-management/deploy-use/log-analyze-usage (https://docs.microsoft.com/rights-management/deploy-use/log-analyze-usage) on the Microsoft documentation site.

## EXAMPLES

### Example 1: Get the log location
```
PS C:\>Get-AadrmUsageLogStorageAccount
```

This command gets the location for your usage logs.

## PARAMETERS

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Set-AadrmUsageLogStorageAccount](.\Set-AadrmUsageLogStorageAccount.md)


