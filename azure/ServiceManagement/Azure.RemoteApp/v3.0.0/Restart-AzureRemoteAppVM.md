---
external help file: Microsoft.WindowsAzure.Commands.RemoteApp.dll-Help.xml
online version: c85588a2-15e3-4b6e-93b6-3b91dbe1a064
schema: 2.0.0
ms.assetid: 22C43C61-83FE-4008-9C74-DD089D7B90E0
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ServiceManagement/Azure.RemoteApp/v3.0.0/Restart-AzureRemoteAppVM.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ServiceManagement/Azure.RemoteApp/v3.0.0/Restart-AzureRemoteAppVM.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Restart-AzureRemoteAppVM

## SYNOPSIS
Restarts a virtual machine in an Azure RemoteApp collection.

## SYNTAX

```
Restart-AzureRemoteAppVM [-CollectionName] <String> [-UserUpn] <String> [[-LogoffMessage] <String>]
 [[-LogoffWaitSeconds] <Int32>] [-Profile <AzureSMProfile>] [-WhatIf] [-Confirm] [<CommonParameters>]
```

## DESCRIPTION
The **Restart-AzureRemoteAppVM** cmdlet restarts a virtual machine in an Azure RemoteApp collection on which the specified user is connected.

## EXAMPLES

### Example 1: Restart a virtual machine
```
PS C:\>Restart-AzureRemoteAppVM -CollectionName "ContosoVNet" -UserUPN "PattiFuller@contoso.com"
```

This command restarts a virtual machine in an Azure RemoteApp collection named Contoso.
The user PattiFuller@contoso.com is connected to the collection which contains this virtual machine.

## PARAMETERS

### -CollectionName
Specifies the name of an Azure RemoteApp collection.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Name

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Confirm
Prompts you for confirmation before running the cmdlet.Prompts you for confirmation before running the cmdlet.

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

### -LogoffMessage
Specifies a warning message shown to users connected to the virtual machine before this cmdlet logs them off.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -LogoffWaitSeconds
Specifies how long this cmdlet waits before it logs users off.
The default value is 60 seconds.

```yaml
Type: Int32
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
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

### -UserUpn
Specifies the user principal name (UPN) of the user for whom this cmdlet restarts the virtual machine.
To obtain virtual machines in the collection and connected UPNs, use the Get-AzureRemoteAppVM cmdlet.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: True (ByPropertyName, ByValue)
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.Shows what would happen if the cmdlet runs.
The cmdlet is not run.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRemoteAppVM](./Get-AzureRemoteAppVM.md)


