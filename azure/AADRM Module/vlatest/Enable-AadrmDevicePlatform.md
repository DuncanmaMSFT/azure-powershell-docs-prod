---
external help file: Microsoft.RightsManagementServices.Online.Admin.PowerShell.dll-Help.xml
online version: http://go.microsoft.com/fwlink/?LinkId=400603
schema: 2.0.0
ms.assetid: 1D21A18B-1E3D-434C-A283-E65B810EF1B4
updated_at: 10/24/2016 10:52 PM
ms.date: 10/24/2016
content_git_url: https://github.com/Azure/azure-docs-powershell-aip/blob/master/Azure%20Information%20Protection/AADRM%20Module/vlatest/Enable-AadrmDevicePlatform.md
gitcommit: https://github.com/Azure/azure-docs-powershell-aip/blob/5e6ef5e3f1d6768f64c5d14aab4fd3e58b8fa0c3/Azure%20Information%20Protection/AADRM%20Module/vlatest/Enable-AadrmDevicePlatform.md
ms.topic: reference
ms.prod: powershell
ms.service: rights-management
ms.technology: Azure Powershell
author: visual-studio-china
keywords: powershell, cmdlet
manager: visual-studio-china
---

# Enable-AadrmDevicePlatform

## SYNOPSIS
Enables Rights Management support for device platforms.

## SYNTAX

### AllPlatforms
```
Enable-AadrmDevicePlatform [-All] [<CommonParameters>]
```

### Platforms
```
Enable-AadrmDevicePlatform [-Windows] [-WindowsStore] [-WindowsPhone] [-Mac] [-iOS] [-Android] [-Web]
 [<CommonParameters>]
```

## DESCRIPTION
The **Enable-AadrmDevicePlatform** cmdlet enables Rights Management support for device platforms.
Your organization can support any combination of the following device platforms: 

- Android
- iOS
- Macintosh operating system
- Web
- Windows operating system
- Windows Phone
- Windows Store

To support all platforms, specify the **All** parameter.

## EXAMPLES

### Example 1: Enable Rights Management support for device platforms
```
PS C:\>Enable-AadrmDevicePlatform -WindowsPhone -WindowStore
```

This command enables Rights Management support for Windows Phone and Windows Store device platforms.

### Example 2: Enable Rights Management support for all device platforms
```
PS C:\>Enable-AadrmDevicePlatform -All
```

This command enables Rights Management support for all device platforms.

## PARAMETERS

### -All
Indicates that the cmdlet specifies all device platforms.
The cmdlet enables Rights Management support for all device platforms.

```yaml
Type: SwitchParameter
Parameter Sets: AllPlatforms
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Android
Indicates that the cmdlet specifies the Android device platform.
The cmdlet enables Rights Management support for the specified device platform.

```yaml
Type: SwitchParameter
Parameter Sets: Platforms
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -iOS
Indicates that the cmdlet specifies the iOS device platform.
The cmdlet enables Rights Management support for the specified device platform.

```yaml
Type: SwitchParameter
Parameter Sets: Platforms
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Mac
Indicates that the cmdlet specifies the Macintosh operating system device platform.
The cmdlet enables Rights Management support for the specified device platform.

```yaml
Type: SwitchParameter
Parameter Sets: Platforms
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Web
Indicates that the cmdlet specifies the web device platform.
The cmdlet enables Rights Management support for the specified device platform.

```yaml
Type: SwitchParameter
Parameter Sets: Platforms
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Windows
Indicates that the cmdlet specifies the Windows operating system device platform.
The cmdlet enables Rights Management support for the specified device platform.

```yaml
Type: SwitchParameter
Parameter Sets: Platforms
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WindowsPhone
Indicates that the cmdlet specifies the Windows Phone device platform.
The cmdlet enables Rights Management support for the specified device platform.

```yaml
Type: SwitchParameter
Parameter Sets: Platforms
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WindowsStore
Indicates that the cmdlet specifies the Windows Store device platform.
The cmdlet enables Rights Management support for the specified device platform.

```yaml
Type: SwitchParameter
Parameter Sets: Platforms
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

## RELATED LINKS

[Disable-AadrmDevicePlatform](./Disable-AadrmDevicePlatform.md)

[Get-AadrmDevicePlatform](./Get-AadrmDevicePlatform.md)


