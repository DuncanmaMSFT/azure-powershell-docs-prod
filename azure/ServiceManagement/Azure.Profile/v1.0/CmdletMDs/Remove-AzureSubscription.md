---
external help file: Microsoft.WindowsAzure.Commands.Profile.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkID=397627
schema: 2.0.0
updated_at: 10/14/2016 7:06 AM
ms.date: 10/14/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Profile/v1.0/CmdletMDs/Remove-AzureSubscription.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/a56d0e01e65c2c33aa2af13dd29addc94ead6e88/azureps-cmdlets-docs/ServiceManagement/Azure.Profile/v1.0/CmdletMDs/Remove-AzureSubscription.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: Visual Studio China
keywords: powershell, content
manager: Visual Studio China
---

# Remove-AzureSubscription

## SYNOPSIS
Deletes an Azure subscription from Windows PowerShell.

## SYNTAX

### Name (Default)
```
Remove-AzureSubscription [-SubscriptionName] <String> [-Force] [-PassThru] [-Profile <AzureSMProfile>]
 [-WhatIf] [-Confirm] [<CommonParameters>]
```

### Id
```
Remove-AzureSubscription [-SubscriptionId] <String> [-Force] [-PassThru] [-Profile <AzureSMProfile>] [-WhatIf]
 [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureSubscription** cmdlet deletes an Azure subscription from your subscription data file so Windows PowerShell can't find it.
This cmdlet does not delete the subscription from Microsoft Azure, or change the actual subscription in any way.

powershell_prelim

## EXAMPLES

### Example 1: Delete a subscription
```
C:\PS> Remove-AzureSubscription -SubscriptionName Test

Confirm
Are you sure you want to perform this action?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "Y"):
```

This command deletes the "Test" subscription from the default subscription data file.

### Example 2: Delete from an alternate subscription data file
```
C:\PS> Remove-AzureSubscription -SubscriptionName Test -SubscriptionDataFile C:\Subs\MySubscriptions.xml -Force
```

This command deletes the Test subscription from the MySubscriptions.xml subscription data file.
The command uses the **Force** parameter to suppress the confirmation prompt.

### Example 3: Delete a subscription in a script
```
C:\PS> ...if (Remove-AzureSubscription -SubscriptionName Test -PassThru) {...}
```

This command uses the **Remove-AzureSubscription** command in an **If** statement.
It uses the **PassThru** parameter, which returns a Boolean value, to determine whether the script block in the **If** statement is executed.

## PARAMETERS

### -SubscriptionName
@{Text=}

```yaml
Type: String
Parameter Sets: Name
Aliases: Name

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Force
@{Text=}

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -PassThru
@{Text=}

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Profile
@{Text=}

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

### -SubscriptionId
@{Text=}

```yaml
Type: String
Parameter Sets: Id
Aliases: Id

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### None
You can pipe input to this cmdlet by property name, but not by value.

## OUTPUTS

### None or System.Boolean
If you use the **PassThru** parameter, this cmdlet returns a Boolean value.
Otherwise, it does not return any output.

## NOTES

## RELATED LINKS

[Get-AzureSubscription](.\Get-AzureSubscription.md)

[Select-AzureSubscription](.\Select-AzureSubscription.md)

[Set-AzureSubscription](.\Set-AzureSubscription.md)
