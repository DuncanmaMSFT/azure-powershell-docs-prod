---
external help file: Microsoft.WindowsAzure.Commands.ServiceManagement.dll-Help.xml
online version: c6e6f7e8-fef9-4f86-8aa0-98d836c68034
schema: 2.0.0
ms.assetid: B0B92619-D674-4E43-89B2-4BD3001140CD
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v3.0.0/Remove-AzureServiceDiagnosticsExtension.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.Service/v3.0.0/Remove-AzureServiceDiagnosticsExtension.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Remove-AzureServiceDiagnosticsExtension

## SYNOPSIS
Removes the cloud service diagnostics extension applied on all roles or named roles at a certain deployment slot.

## SYNTAX

### RemoveByRoles (Default)
```
Remove-AzureServiceDiagnosticsExtension [[-ServiceName] <String>] [[-Slot] <String>] [[-Role] <String[]>]
 [-Profile <AzureSMProfile>] [<CommonParameters>]
```

### RemoveAllRoles
```
Remove-AzureServiceDiagnosticsExtension [[-ServiceName] <String>] [[-Slot] <String>] [-UninstallConfiguration]
 [-Profile <AzureSMProfile>] [<CommonParameters>]
```

## DESCRIPTION
The **Remove-AzureServiceDiagnosticsExtension** cmdlet removes the cloud service diagnostics extension applied on all roles or named roles at a certain deployment slot.

## EXAMPLES

### Example 1: Remove the diagnostic extension for a service
```
PS C:\>Remove-AzureServiceDiagnosticsExtension -ServiceName $Svc
```

This command removes the diagnostic extension for a specified role.

### Example 2: Remove the diagnostic extension for a service in a specified role
```
PS C:\>Remove-AzureServiceDiagnosticsExtension -ServiceName $Svc -Role "WebRole01"
```

This command removes the diagnostic extension for a specified role.

## PARAMETERS

### -ServiceName
Specifies the Azure service name of the deployment.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Slot
Specifies the environment of the deployment to modify.
Valid values are Production or Staging.

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

### -Role
Specifies an optional array of roles for which to specify the remote desktop configuration.
If you do not specify this parameter, the remote desktop configuration is applied as the default configuration for all roles.

```yaml
Type: String[]
Parameter Sets: RemoveByRoles
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Profile
Specifies the Azure profile from which this cmdlet reads.
If you do not specify a profile, this cmdlet reads from the local default profile.

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

### -UninstallConfiguration
Indicates that this cmdlet uninstalls all RDP configurations from the cloud service.

```yaml
Type: SwitchParameter
Parameter Sets: RemoveAllRoles
Aliases: 

Required: True
Position: 2
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

[Get-AzureServiceDiagnosticsExtension](./Get-AzureServiceDiagnosticsExtension.md)

[Set-AzureServiceDiagnosticsExtension](./Set-AzureServiceDiagnosticsExtension.md)


