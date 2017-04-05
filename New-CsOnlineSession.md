---
external help file: SkypeOnlineConnectorStartup-help.xml
online version: 
schema: 2.0.0
---

# New-CsOnlineSession

## SYNOPSIS
Creates a persistent connection to Microsoft Lync Online DataCenter.

## SYNTAX

```
New-CsOnlineSession [-Credential] <PSCredential> [[-OverrideAdminDomain] <String>]
 [[-OverrideDiscoveryUri] <Uri>] [[-OverridePowershellUri] <Uri>] [[-SessionOption] <PSSessionOption>]
```

## DESCRIPTION
Creates a remote session to Microsoft Lync Online DataCenter.
In this session, tenant administrator can run Lync cmdlets to manage users, policies and configurations.

## EXAMPLES

### -------------------------- EXAMPLE 1 --------------------------
```
New-CsOnlineSession -Credential User@Domain.com
```

Establishes a Lync Remote PowerShell Session, supplying the credentials of an administrator account of the tenant.

### -------------------------- EXAMPLE 2 --------------------------
```
New-CsOnlineSession -Credential User@Domain.com -OverrideAdminDomain TargetDomain.com
```

Establishes a Lync Remote PowerShell Session, with an administrator account that has permission to manage the tenant TargetDomain.com. 
Please change the OverrideAdminDomain to your target Tenant domain.

## PARAMETERS

### -Credential
Specifies a user account that is Tenant Administrator, or Syndicated Partner Administrator.

Type a user name, such as "User@Domain.com", or enter a PSCredential object, such as one returned by the Get-Credential cmdlet.

When you type a user name, you will be prompted for a password.

```yaml
Type: PSCredential
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OverrideAdminDomain
Specifies a domain to be managed.
This could be home domain of signed in user, or a different one that he/she has permission to manage.
Optional.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OverrideDiscoveryUri
Specifies Lync Auto Discovery URI.
Optional.

```yaml
Type: Uri
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OverridePowershellUri
Specifies Lync Remote Powershell URI.
Optional.

```yaml
Type: Uri
Parameter Sets: (All)
Aliases: 

Required: False
Position: 4
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -SessionOption
Sets advanced options for the session.
Enter a SessionOption object, such as one that you create by using the New-PSSessionOption cmdlet, or a hash table in which the keys are session option names and the values are session option values.

```yaml
Type: PSSessionOption
Parameter Sets: (All)
Aliases: 

Required: False
Position: 5
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

