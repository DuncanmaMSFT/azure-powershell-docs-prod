---
external help file: Microsoft.Azure.Commands.Compute.dll-Help.xml
online version: 975161a1-b1b4-446a-b499-0ea209f02f78
schema: 2.0.0
ms.assetid: A052C39E-360C-4576-94C8-7EAD4D78CBEC
updated_at: 10/24/2016 11:55 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.2.0/New-AzureRmVmssVaultCertificateConfig.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/4377291ee360e58e2c1c5d644155daf6a0279055/azureps-cmdlets-docs/ResourceManager/AzureRM.Compute/v2.2.0/New-AzureRmVmssVaultCertificateConfig.md
ms.topic: reference
ms.prod: powershell
ms.service: azure-powershell
ms.technology: Azure PowerShell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# New-AzureRmVmssVaultCertificateConfig

## SYNOPSIS
Creates a Key Vault certificate configuration.

## SYNTAX

```
New-AzureRmVmssVaultCertificateConfig [[-CertificateUrl] <String>] [[-CertificateStore] <String>]
 [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureRmVmssVaultCertificateConfig** cmdlet specifies the secret that needs to be placed on the Virtual Machine Scale Set (VMSS) virtual machines.
The output of this cmdlet is intended to be used with the Add-AzureRmVmssSecret cmdlet.

## EXAMPLES

### Example 1: Create a Key Vault certificate configuration
```
PS C:\>New-AzureRmVmssVaultCertificateConfig -CertificateUrl "http://keyVaultName.vault.contoso.net/secrets/secretName/secretVersion" -CertificateStore "MyCerts"
```

This command creates a Key Vault certificate configuration that uses the certificate store named MyCerts located at the specified certificate URL.

## PARAMETERS

### -CertificateStore
Specifies the certificate store on the virtual machines in the scale set where the certificate is added.
This is only valid for Windows Virtual Machine Scale Sets.

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

### -CertificateUrl
Specifies the URI of a certificate stored in the Key Vault.

It is the base64 encoding of the following JSON Object which is encoded in UTF-8:

{
  "data":"\<Base64-encoded-certificate\>",
  "dataType":"pfx",
  "password":"\<pfx-file-password\>"
}

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

###  
This cmdlet does not generate any output.

## NOTES

## RELATED LINKS

[Add-AzureRmVmssSecret](./Add-AzureRmVmssSecret.md)


