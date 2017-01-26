---
author: brianlic-msft-msft
description: 
external help file: Microsoft.IdentityServer.Management.dll-Help.xml
keywords: powershell, cmdlet
manager: alanth
ms.date: 2016-12-20
ms.prod: powershell
ms.technology: powershell
ms.topic: reference
online version: 
schema: 2.0.0
title: Get-AdfsWebTheme
ms.assetid: 4C4A7B48-C442-4528-B980-CD6B5E6AEA72
---

# Get-AdfsWebTheme

## SYNOPSIS
Gets web themes.

## SYNTAX

```
Get-AdfsWebTheme [-Name <String>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-AdfsWebTheme** cmdlet gets **AdfsWebTheme** objects.
Specify a web theme by name.
If you do not specify a name, the cmdlet gets all the **AdfsWebTheme** objects.

## EXAMPLES

### Example 1: Get all web themes
```
PS C:\> Get-AdfsWebTheme
Name                    : Default
IsBuiltinTheme          : True
StyleSheet              : {[, System.Byte[]]}
RTLStyleSheet           : {42, 32, 123, 13...}
Logo                    : {[, System.Byte[]]}
Illustration            : {[, System.Byte[]]}
AdditionalFileResources : {[/adfs/portal/script/onload.js, System.Byte[]], [/adfs/portal/images/idp/localsts.png, System.Byte[]], [/adfs/portal/images/idp/idp.png,
System.Byte[]], [/adfs/portal/images/idp/otherorganizations.png, System.Byte[]]}
```

This command gets all the available web themes in Active Directory Federation Services (AD FS).

### Example 2: Get a named web theme
```
PS C:\> Get-AdfsWebTheme -Name "Theme01"
Name                    : Theme01
IsBuiltinTheme          : False
StyleSheet              : {[, System.Byte[]]}
RTLStyleSheet           : {42, 32, 123, 13...}
Logo                    : {[, System.Byte[]]}
Illustration            : {[, System.Byte[]]}
AdditionalFileResources : {[/adfs/portal/script/onload.js, System.Byte[]], [/adfs/portal/images/idp/localsts.png, System.Byte[]], [/adfs/portal/images/idp/idp.png,
System.Byte[]], [/adfs/portal/images/idp/otherorganizations.png, System.Byte[]]}
```

This command gets the theme named Theme01.

## PARAMETERS

### -Name
Specifies a name.
The cmdlet gets the web theme that has the name that you specify.

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

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

### System.String

## OUTPUTS

### Microsoft.IdentityServer.Management.Resources.AdfsWebTheme;Microsoft.IdentityServer.Management.Resources.AdfsWebTheme[]
This cmdlet generates a web customization object, **System.IdentityServer.Management.Resources.AdfsWebTheme**, or an array of these objects.
This object includes the following properties: 

Name: **System.String**
IsBuiltinTheme: **System.Boolean**
StyleSheet: **IDictionary\<CultureInfo, byte\[\]\>**
RTLStyleSheet: **byte\[\]**
Logo: **IDictionary\<CultureInfo, byte\[\]\>**
Illustration: **IDictionary\<CultureInfo, byte\[\]\>**
AdditionalFileResources: **IDictionary\<string, byte\[\]\>**

## NOTES

## RELATED LINKS

[Export-AdfsWebTheme](./Export-AdfsWebTheme.md)

[New-AdfsWebTheme](./New-AdfsWebTheme.md)

[Remove-AdfsWebTheme](./Remove-AdfsWebTheme.md)

[Set-AdfsWebTheme](./Set-AdfsWebTheme.md)
