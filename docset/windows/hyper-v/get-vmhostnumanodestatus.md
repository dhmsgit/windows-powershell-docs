---
ms.mktglfcycl: manage
ms.sitesec: library
ms.author: brianlic
author: brianlic-msft
description: Use this topic to help manage Windows and Windows Server technologies with Windows PowerShell.
external help file: Microsoft.HyperV.PowerShell.Cmdlets.dll-Help.xml
keywords: powershell, cmdlet
manager: alanth
ms.date: 2016-12-20
ms.prod: w10
ms.technology: powershell-windows
ms.topic: reference
online version: 
schema: 2.0.0
title: Get-VMHostNumaNodeStatus
ms.assetid: F9F5EB63-5D14-4862-BC04-4FB93BFC5855
---

# Get-VMHostNumaNodeStatus

## SYNOPSIS
Gets the status of the virtual machines on the non-uniform memory access (NUMA) nodes of a virtual machine host or hosts.

## SYNTAX

### ComputerName (Default)
```
Get-VMHostNumaNodeStatus [[-ComputerName] <String[]>] [[-Credential] <PSCredential[]>] [-Id <Int32>]
 [<CommonParameters>]
```

### CimSession
```
Get-VMHostNumaNodeStatus [-CimSession] <CimSession[]> [-Id <Int32>] [<CommonParameters>]
```

## DESCRIPTION
The **Get-VMHostNumaNodeStatus** cmdlet gets the status of the virtual machines on the non-uniform memory access (NUMA) nodes of a virtual machine host or hosts.
If the virtual machine host enables NUMA spanning, this cmdlet returns an error.

## EXAMPLES

### Example 1
```
PS C:\> Get-VMHostNumaNodeStatus
```

Gets the status of the virtual machines on the non-uniform memory access (NUMA) nodes of the local Hyper-V host.

## PARAMETERS

### -CimSession
Runs the cmdlet in a remote session or on a remote computer.
Enter a computer name or a session object, such as the output of a [New-CimSession](http://go.microsoft.com/fwlink/p/?LinkId=227967) or [Get-CimSession](http://go.microsoft.com/fwlink/p/?LinkId=227966) cmdlet.
The default is the current session on the local computer.

```yaml
Type: CimSession[]
Parameter Sets: CimSession
Aliases: 

Required: True
Position: 0
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ComputerName
Specifies one or more Hyper-V hosts that run this cmdlet.
NetBIOS names, IP addresses, and fully qualified domain names are allowable.
The default is the local computer.
Use localhost or a dot (.) to specify the local computer explicitly.

```yaml
Type: String[]
Parameter Sets: ComputerName
Aliases: 

Required: False
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Credential
Specifies one or more user accounts that have permission to perform this action.
The default is the current user.

```yaml
Type: PSCredential[]
Parameter Sets: ComputerName
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Id
Identifies a NUMA node for which virtual machine status is to be retrieved.

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
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see [about_CommonParameters](http://go.microsoft.com/fwlink/?LinkID=113216).

## INPUTS

## OUTPUTS

### VMNumaNodeStatus[]

## NOTES

## RELATED LINKS

