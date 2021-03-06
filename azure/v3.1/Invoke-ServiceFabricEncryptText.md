---
external help file: Microsoft.ServiceFabric.Powershell.dll-Help.xml
online version: 
schema: 2.0.0
updated_at: 10/18/2016 3:10 PM
ms.date: 10/18/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/master/ServiceFabric/v3.1/Invoke-ServiceFabricEncryptText.md
gitcommit: https://github.com/Azure/azure-docs-powershell-servicefabric/blob/64b91ee622d0b9ae6539db10e927e50881fae64d/ServiceFabric/v3.1/Invoke-ServiceFabricEncryptText.md
ms.topic: reference
ms.prod: powershell
ms.service: service-fabric
ms.technology: Azure Powershell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Invoke-ServiceFabricEncryptText

## SYNOPSIS
{{Fill in the Synopsis}}

## SYNTAX

### CertStore
```
Invoke-ServiceFabricEncryptText [-Text] <String> [-AlgorithmOid <String>] [-CertStore] -CertThumbprint <String>
 [-StoreName <String>] [-StoreLocation <StoreLocation>] [-TimeoutSec <Int32>] [<CommonParameters>]
```

### CertFile
```
Invoke-ServiceFabricEncryptText [-Text] <String> [-AlgorithmOid <String>] [-CertFile] -Path <String>
 [-TimeoutSec <Int32>] [<CommonParameters>]
```

## DESCRIPTION
{{Fill in the Description}}

## EXAMPLES

### Example 1
```
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -AlgorithmOid
Cryptographic object identifier of encryption algorithm to use, for example, "2.16.840.1.101.3.4.1.42" is AES-256-CBC

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CertFile
Load encryption certificate from a file, supported format: DER encoded binary X509 (.CER)

```yaml
Type: SwitchParameter
Parameter Sets: CertFile
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CertStore
Load encryption certificate from certificate store

```yaml
Type: SwitchParameter
Parameter Sets: CertStore
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CertThumbprint
Thumbprint of encryption certificate

```yaml
Type: String
Parameter Sets: CertStore
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Path
Path of encryption certificate file

```yaml
Type: String
Parameter Sets: CertFile
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StoreLocation
Certificate store location, default to LocalMachine

```yaml
Type: StoreLocation
Parameter Sets: CertStore
Aliases: 
Accepted values: CurrentUser, LocalMachine

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -StoreName
Certificate store name, default to "My"

```yaml
Type: String
Parameter Sets: CertStore
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Text
Text to encrypt

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -TimeoutSec
{{Fill TimeoutSec Description}}

```yaml
Type: Int32
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

### None

## OUTPUTS

### System.Object

## NOTES

## RELATED LINKS

