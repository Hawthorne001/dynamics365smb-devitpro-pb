---
title: "RecordRef.CurrentKey() Method"
description: "Gets the current key of the table referred to by the RecordRef."
ms.author: solsen
ms.date: 08/26/2024
ms.topic: reference
author: SusanneWindfeldPedersen
ms.reviewer: solsen
---
[//]: # (START>DO_NOT_EDIT)
[//]: # (IMPORTANT:Do not edit any of the content between here and the END>DO_NOT_EDIT.)
[//]: # (Any modifications should be made in the .xml files in the ModernDev repo.)
# RecordRef.CurrentKey() Method
> **Version**: _Available or changed with runtime version 1.0._

Gets the current key of the table referred to by the RecordRef. The current key is returned as a string.


## Syntax
```AL
CurrentKey :=   RecordRef.CurrentKey()
```
> [!NOTE]
> This method can be invoked using property access syntax.
## Parameters
*RecordRef*  
&emsp;Type: [RecordRef](recordref-data-type.md)  
An instance of the [RecordRef](recordref-data-type.md) data type.  

## Return Value
*CurrentKey*  
&emsp;Type: [Text](../text/text-data-type.md)  
The name of the current key of the record.


[//]: # (IMPORTANT: END>DO_NOT_EDIT)

## Example  

```al
var
    RecRef: RecordRef;
    Text000: Label 'The current key in the "%1" table is "%2".';
begin
    RecRef.Open(18);  
    Message(Text000,RecRef.Caption,RecRef.CurrentKey);
end;  
```  
  
 `RecRef.Open(18)` - Opens table 18 or causes a runtime error if table 18 doesn't exist.  
  
 `RecRef.Caption` - Returns the caption of the table.  
  
 `RecRef.CurrentKey` - Returns the caption of the current key in the table.  
  
## Related information
[RecordRef Data Type](recordref-data-type.md)  
[Get Started with AL](../../devenv-get-started.md)  
[Developing Extensions](../../devenv-dev-overview.md)