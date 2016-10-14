---
external help file: Microsoft.Azure.Commands.Websites.dll-Help.xml
online version: .\Get-AzureRmWebAppSSLBinding.md
schema: 2.0.0
updated_at: 10/14/2016 7:06 AM
ms.date: 10/14/2016
content_git_url: https://github.com/Azure/azure-docs-powershell/blob/master/azureps-cmdlets-docs/ResourceManager/AzureRM.Websites/v1.0/CmdletMDs/New-AzureRmWebAppSSLBinding.md
gitcommit: https://github.com/Azure/azure-docs-powershell/blob/a56d0e01e65c2c33aa2af13dd29addc94ead6e88/azureps-cmdlets-docs/ResourceManager/AzureRM.Websites/v1.0/CmdletMDs/New-AzureRmWebAppSSLBinding.md
ms.topic: reference
ms.prod: powershell
ms.service: Azure PowerShell
ms.technology: Azure PowerShell
author: Visual Studio China
keywords: powershell, content
manager: Visual Studio China
---

# New-AzureRmWebAppSSLBinding

## SYNOPSIS
Creates an SSL certificate binding for an azure_2 Web App.

## SYNTAX

### S2
```
New-AzureRmWebAppSSLBinding [-ResourceGroupName] <String> [-WebAppName] <String> [[-Slot] <String>]
 [-Name] <String> [[-SslState] <SslState>] [-Thumbprint] <String> [<CommonParameters>]
```

### S1
```
New-AzureRmWebAppSSLBinding [-ResourceGroupName] <String> [-WebAppName] <String> [[-Slot] <String>]
 [-Name] <String> [[-SslState] <SslState>] [-CertificateFilePath] <String> [-CertificatePassword] <String>
 [<CommonParameters>]
```

### S3
```
New-AzureRmWebAppSSLBinding [-WebApp] <Site> [-Name] <String> [[-SslState] <SslState>]
 [-CertificateFilePath] <String> [-CertificatePassword] <String> [<CommonParameters>]
```

### S4
```
New-AzureRmWebAppSSLBinding [-WebApp] <Site> [-Name] <String> [[-SslState] <SslState>] [-Thumbprint] <String>
 [<CommonParameters>]
```

## DESCRIPTION
The **New-AzureRmWebAppSSLBinding** cmdlet creates a Secure Socket Layer (SSL) certificate binding for an azure_2 Web App.
The cmdlet creates an SSL binding in two ways: 

- You can bind a Web App to an existing certificate.
- You can upload a new certificate and then bind the Web App to this new certificate.

Regardless of which approach you use, the certificate and the Web App must be associated with the same azure_2 resource group.
If you have a Web App in Resource Group A and you want to bind that Web App to a certificate in Resource Group B, the only way to do that is to upload a copy of the certificate to Resource Group A.

If you upload a new certificate, keep in mind the following requirements for an azure_2 SSL certificate: 

- The certificate must contain a private key. 
- The certificate must use the Personal Information Exchange (PFX) format. 
- The certificate's subject name must match the domain used to access the Web App. 
- The certificate must use a minimum of 2048-bit encryption.

## EXAMPLES

### Example 1: Bind a certificate to a Web App
```
PS C:\>New-AzureRmWebAppSSLBinding -ResourceGroupName "ContosoResourceGroup" -WebAppName "ContosoWebApp" -Thumbprint "E3A38EBA60CAA1C162785A2E1C44A15AD450199C3" -Name "www.contoso.com" -CertificatePassword "p@ssw0rd"
```

This command binds an existing azure_2 certificate (a certificate with the Thumbprint E3A38EBA60CAA1C162785A2E1C44A15AD450199C3) to the web app named ContosoWebApp.

### Example 2: Upload a certificate and bind it to a Web App
```
PS C:\>New-AzureRmWebAppSSLBinding -ResourceGroupName "ContosoResourceGroup" -WebAppName "ContosoWebApp" -Thumbprint "E3A38EBA60CAA1C162785A2E1C44A15AD450199C3" -Name "www.contoso.com" -CertificatePassword "p@ssw0rd" -CertificateFilePath "C:\Certificates\ContosoWebSite.pfx"
```

Example 2 also binds the certificate E3A38EBA60CAA1C162785A2E1C44A15AD450199C3 to the Web App named ContosoWebApp.
In this case, however, the certificate has not yet been uploaded to azure_2.
Because of that, the *CertificateFilePath* parameter is used to specify the local copy of the certificate .PFX file.
This certificate will be uploaded to azure_2 and then the new SSL bindings will be created.

## PARAMETERS

### -ResourceGroupName
Specifies the name of the resource group that the certificate is assigned to.

You cannot use the *ResourceGroupName* parameter and the *WebApp* parameter in the same command.

```yaml
Type: String
Parameter Sets: S2, S1
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WebAppName
Specifies the name of the Web App for which the new SSL binding is being created.

You cannot use the *WebAppName* parameter and the *WebApp* parameter in the same command.

```yaml
Type: String
Parameter Sets: S2, S1
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Slot
Specifies the name of the Web App deployment slot.
You can use the Get-AzureRMWebAppSlot cmdlet to get a slot.

Deployment slots provide a way for you to stage and validate web apps without those apps being accessible over the Internet.
Typically you will deploy your changes to a staging site, validate those changes, and then deploy to the production (Internet-accessible) site.

```yaml
Type: String
Parameter Sets: S2, S1
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Name
Specifies the name of the Web App.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SslState
Specifies whether the certificate is enabled.
Set the *SSLState* parameter to 1 to enable the certificate, or set *SSLState* to 0 to disable the certificate.

```yaml
Type: SslState
Parameter Sets: (All)
Aliases: 

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Thumbprint
Specifies the unique identifier for the certificate.

```yaml
Type: String
Parameter Sets: S2, S4
Aliases: 

Required: True
Position: 6
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CertificateFilePath
Specifies the file path for the certificate to be uploaded.

The *CertificateFilePath* parameter is only required if the certificate has not yet been uploaded to azure_2.

```yaml
Type: String
Parameter Sets: S1, S3
Aliases: 

Required: True
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CertificatePassword
Specifies the decryption password for the certificate.

```yaml
Type: String
Parameter Sets: S1, S3
Aliases: 

Required: True
Position: 5
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WebApp
Specifies a Web App.
To get a Web App, use the Get-AzureRmWebApp cmdlet.

You cannot use the *WebApp* parameter in the same command as the *ResourceGroupName* parameter and/or the *WebAppName*.

```yaml
Type: Site
Parameter Sets: S3, S4
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[Get-AzureRmWebAppSSLBinding](.\Get-AzureRmWebAppSSLBinding.md)

[Remove-AzureRmWebAppSSLBinding](.\Remove-AzureRmWebAppSSLBinding.md)

[Get-AzureRMWebAppSlot](.\Get-AzureRMWebAppSlot.md)

[Get-AzureRmWebApp](.\Get-AzureRmWebApp.md)
