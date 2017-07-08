---
external help file: Microsoft.AzureStack.AzureConsistentStorage.Commands.dll-Help.xml
online version: 
schema: 2.0.0
---

# Get-AzsStorageShareMetricDefinition

## SYNOPSIS
Gets the properties of the metric definitions exposed at the share level.

## SYNTAX

```
Get-AzsStorageShareMetricDefinition -ShareName <String> [-MetricNames <String[]>] [-DetailedOutput]
 [-SkipCertificateValidation]
```

## DESCRIPTION
The **Get-AzsStorageShareMetricDefinition** cmdlet gets the properties of the metric definitions exposed at the share level.

## EXAMPLES

```
$shares = Get-AzsStorageShare

Get-AzsStorageShareMetricDefinition -ShareName $shares[0].ShareName -DetailedOutput | Format-Table -Wrap 

```

## PARAMETERS

### -DetailedOutput
Indicates the cmdlet gets the detailed metric definitions from the Azs Share.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -MetricNames
Specifies a string array of metric names in which this cmdlet gets definitions from.

```yaml
Type: String[]
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ShareName
Specifies the name of the Azs share that this cmdlet gets.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -SkipCertificateValidation
Indicates that the cmdlet does not validate the certificate.

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
### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (http://go.microsoft.com/fwlink/?LinkID=113216).

## RELATED LINKS

[Get-AzsStorageShare](./Get-AzsStorageShare.md)

[Get-AzsStorageShareMetric](./Get-AzsStorageShareMetric.md)
