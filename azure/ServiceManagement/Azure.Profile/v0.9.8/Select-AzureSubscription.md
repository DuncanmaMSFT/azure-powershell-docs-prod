---
external help file: Microsoft.WindowsAzure.Commands.Profile.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkID=397628
schema: 2.0.0
ms.assetid: 3F21DAF8-995D-4DA4-BB2F-CED48DC39772
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Profile/v0.9.8/Select-AzureSubscription.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.Profile/v0.9.8/Select-AzureSubscription.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Select-AzureSubscription

## SYNOPSIS
Changes the current and default Azure subscriptions

## SYNTAX

### SelectSubscriptionByNameParameterSet (Default)
```
Select-AzureSubscription [-SubscriptionName] <String> [[-Account] <String>] [-Current] [-PassThru]
 [-Profile <AzureProfile>] [<CommonParameters>]
```

### SelectDefaultSubscriptionByNameParameterSet
```
Select-AzureSubscription [-SubscriptionName] <String> [[-Account] <String>] [-Default] [-PassThru]
 [-Profile <AzureProfile>] [<CommonParameters>]
```

### SelectSubscriptionByIdParameterSet
```
Select-AzureSubscription [-SubscriptionId] <String> [[-Account] <String>] [-Current] [-PassThru]
 [-Profile <AzureProfile>] [<CommonParameters>]
```

### SelectDefaultSubscriptionByIdParameterSet
```
Select-AzureSubscription [-SubscriptionId] <String> [[-Account] <String>] [-Default] [-PassThru]
 [-Profile <AzureProfile>] [<CommonParameters>]
```

### NoCurrentSubscriptionParameterSet
```
Select-AzureSubscription [[-Account] <String>] [-NoCurrent] [-PassThru] [-Profile <AzureProfile>]
 [<CommonParameters>]
```

### NoDefaultSubscriptionParameterSet
```
Select-AzureSubscription [[-Account] <String>] [-NoDefault] [-PassThru] [-Profile <AzureProfile>]
 [<CommonParameters>]
```

## DESCRIPTION
The **Select-AzureSubscription** cmdlet sets and clears the current and default Azure subscriptions.

The "current subscription" is the subscription that is used by default in the current Windows PowerShell session.
The "default subscription" is used by default in all Windows PowerShell sessions.
The "current subscription" label lets you specify a different subscription to be used by default for the current session without changing the "default subscription" for all other sessions.

The "default" subscription designation is saved in your subscription data file.
The session-specific "current" designation is not saved.

This topic describes the cmdlet in the 0.8.10 version of the Microsoft Azure PowerShell module.
To get the version of the module you're using, in the Azure PowerShell console, type (Get-Module -Name Azure).Version.

## EXAMPLES

### Example 1: Set the current subscription
```
C:\PS> Select-AzureSubscription -Current -SubscriptionName ContosoEngineering
```

This command makes "ContosoEngineering" the current subscription.

### Example 2: Set the default description
```
C:\PS> Select-AzureSubscription -Default -SubscriptionName ContosoFinance -SubscriptionDataFile "C:\subs\MySubscriptions.xml"
```

This command changes the default subscription to "ContosoFinance." It saves the setting in the Subscriptions.xml subscription data file, instead of the default subscription data file.

## PARAMETERS

### -SubscriptionName
@{Text=}

```yaml
Type: String
Parameter Sets: SelectSubscriptionByNameParameterSet, SelectDefaultSubscriptionByNameParameterSet
Aliases: Name

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Account
@{Text=}

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Current
@{Text=}

```yaml
Type: SwitchParameter
Parameter Sets: SelectSubscriptionByNameParameterSet, SelectSubscriptionByIdParameterSet
Aliases: 

Required: False
Position: Named
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
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Profile
@{Text=}

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

### -Default
@{Text=}

```yaml
Type: SwitchParameter
Parameter Sets: SelectDefaultSubscriptionByNameParameterSet, SelectDefaultSubscriptionByIdParameterSet
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SubscriptionId
@{Text=}

```yaml
Type: String
Parameter Sets: SelectSubscriptionByIdParameterSet, SelectDefaultSubscriptionByIdParameterSet
Aliases: Id

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -NoCurrent
@{Text=}

```yaml
Type: SwitchParameter
Parameter Sets: NoCurrentSubscriptionParameterSet
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -NoDefault
@{Text=}

```yaml
Type: SwitchParameter
Parameter Sets: NoDefaultSubscriptionParameterSet
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
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
By default, it does not generate any output.

## NOTES

## RELATED LINKS

[Get-AzureSubscription](./Get-AzureSubscription.md)

[Remove-AzureSubscription](./Remove-AzureSubscription.md)

[Set-AzureSubscription](./Set-AzureSubscription.md)


