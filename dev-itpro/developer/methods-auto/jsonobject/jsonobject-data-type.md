---
title: "JsonObject data type"
description: "Is a container for any well-formed JSON object."
ms.author: solsen
ms.date: 06/10/2025
ms.topic: reference
author: SusanneWindfeldPedersen
ms.reviewer: solsen
---
[//]: # (START>DO_NOT_EDIT)
[//]: # (IMPORTANT:Do not edit any of the content between here and the END>DO_NOT_EDIT.)
[//]: # (Any modifications should be made in the .xml files in the ModernDev repo.)
# JsonObject data type
> **Version**: _Available or changed with runtime version 1.0._

Is a container for any well-formed JSON object. A default JsonObject contains an empty JSON object.



## Instance methods
The following methods are available on instances of the JsonObject data type.

|Method name|Description|
|-----------|-----------|
|[Add(Text, JsonToken)](jsonobject-add-string-jsontoken-method.md)|Adds a new property to a JsonObject.|
|[Add(Text, JsonObject)](jsonobject-add-string-jsonobject-method.md)|Adds a new property to a JsonObject.|
|[Add(Text, JsonValue)](jsonobject-add-string-jsonvalue-method.md)|Adds a new property to a JsonObject.|
|[Add(Text, JsonArray)](jsonobject-add-string-jsonarray-method.md)|Adds a new property to a JsonObject.|
|[Add(Text, Boolean)](jsonobject-add-string-boolean-method.md)|Adds a new property to a JsonObject.|
|[Add(Text, Char)](jsonobject-add-string-char-method.md)|Adds a new property to a JsonObject.|
|[Add(Text, Byte)](jsonobject-add-string-byte-method.md)|Adds a new property to a JsonObject.|
|[Add(Text, Option)](jsonobject-add-string-option-method.md)|Adds a new property to a JsonObject.|
|[Add(Text, Integer)](jsonobject-add-string-integer-method.md)|Adds a new property to a JsonObject.|
|[Add(Text, BigInteger)](jsonobject-add-string-biginteger-method.md)|Adds a new property to a JsonObject.|
|[Add(Text, Decimal)](jsonobject-add-string-decimal-method.md)|Adds a new property to a JsonObject.|
|[Add(Text, Duration)](jsonobject-add-string-duration-method.md)|Adds a new property to a JsonObject.|
|[Add(Text, Text)](jsonobject-add-string-string-method.md)|Adds a new property to a JsonObject.|
|[Add(Text, Date)](jsonobject-add-string-date-method.md)|Adds a new property to a JsonObject.|
|[Add(Text, Time)](jsonobject-add-string-time-method.md)|Adds a new property to a JsonObject.|
|[Add(Text, DateTime)](jsonobject-add-string-datetime-method.md)|Adds a new property to a JsonObject.|
|[AsToken()](jsonobject-astoken-method.md)|Converts the value in a JsonObject to a JsonToken data type.|
|[Clone()](jsonobject-clone-method.md)|Creates a deep-copy of the JsonToken value.|
|[Contains(Text)](jsonobject-contains-method.md)|Verifies if a JsonObject contains a property with a given key.|
|[Get(Text, var JsonToken)](jsonobject-get-method.md)|Retrieves the value of a property with a given key from a JsonObject.|
|[GetArray(Text [, Boolean])](jsonobject-getarray-method.md)|Retrieves the value of a property with a given key from a JsonObject as a JsonArray.|
|[GetBigInteger(Text [, Boolean])](jsonobject-getbiginteger-method.md)|Retrieves the value of a property with a given key from a JsonObject as a BigInteger.|
|[GetBoolean(Text [, Boolean])](jsonobject-getboolean-method.md)|Retrieves the value of a property with a given key from a JsonObject as a Boolean.|
|[GetByte(Text [, Boolean])](jsonobject-getbyte-method.md)|Retrieves the value of a property with a given key from a JsonObject as a Byte.|
|[GetChar(Text [, Boolean])](jsonobject-getchar-method.md)|Retrieves the value of a property with a given key from a JsonObject as a Char.|
|[GetDate(Text [, Boolean])](jsonobject-getdate-method.md)|Retrieves the value of a property with a given key from a JsonObject as a Date.|
|[GetDateTime(Text [, Boolean])](jsonobject-getdatetime-method.md)|Retrieves the value of a property with a given key from a JsonObject as a DateTime.|
|[GetDecimal(Text [, Boolean])](jsonobject-getdecimal-method.md)|Retrieves the value of a property with a given key from a JsonObject as an Decimal.|
|[GetDuration(Text [, Boolean])](jsonobject-getduration-method.md)|Retrieves the value of a property with a given key from a JsonObject as a Duration.|
|[GetInteger(Text [, Boolean])](jsonobject-getinteger-method.md)|Retrieves the value of a property with a given key from a JsonObject as an Integer.|
|[GetObject(Text [, Boolean])](jsonobject-getobject-method.md)|Retrieves the value of a property with a given key from a JsonObject as a JsonObject.|
|[GetOption(Text [, Boolean])](jsonobject-getoption-method.md)|Retrieves the value of a property with a given key from a JsonObject as an Option.|
|[GetText(Text [, Boolean])](jsonobject-gettext-method.md)|Retrieves the value of a property with a given key from a JsonObject as Text.|
|[GetTime(Text [, Boolean])](jsonobject-gettime-method.md)|Retrieves the value of a property with a given key from a JsonObject as a Time.|
|[Keys()](jsonobject-keys-method.md)|Gets a set of keys of the JsonObject.|
|[Path()](jsonobject-path-method.md)|Retrieves the JSON path of the object relative to the root of its containing tree.|
|[ReadFrom(Text)](jsonobject-readfrom-string-method.md)|Reads the JSON data from the string into a JsonObject variable.|
|[ReadFrom(InStream)](jsonobject-readfrom-instream-method.md)|Reads the JSON data from the stream into a JsonObject variable.|
|[ReadFromYaml(Text)](jsonobject-readfromyaml-string-method.md)|Reads the YAML data from the string into a JsonObject variable.|
|[ReadFromYaml(InStream)](jsonobject-readfromyaml-instream-method.md)|Reads the YAML data from the stream into a JsonObject variable.|
|[Remove(Text)](jsonobject-remove-method.md)|Removes the property with the given key from the object.|
|[Replace(Text, JsonToken)](jsonobject-replace-string-jsontoken-method.md)|Replaces the value of the property with the given key with the new value.|
|[Replace(Text, JsonArray)](jsonobject-replace-string-jsonarray-method.md)|Replaces the value of the property with the given key with the new value.|
|[Replace(Text, JsonObject)](jsonobject-replace-string-jsonobject-method.md)|Replaces the value of the property with the given key with the new value.|
|[Replace(Text, JsonValue)](jsonobject-replace-string-jsonvalue-method.md)|Replaces the value of the property with the given key with the new value.|
|[Replace(Text, Boolean)](jsonobject-replace-string-boolean-method.md)|Replaces the value of the property with the given key with the new value.|
|[Replace(Text, Char)](jsonobject-replace-string-char-method.md)|Replaces the value of the property with the given key with the new value.|
|[Replace(Text, Byte)](jsonobject-replace-string-byte-method.md)|Replaces the value of the property with the given key with the new value.|
|[Replace(Text, Integer)](jsonobject-replace-string-integer-method.md)|Replaces the value of the property with the given key with the new value.|
|[Replace(Text, Option)](jsonobject-replace-string-option-method.md)|Replaces the value of the property with the given key with the new value.|
|[Replace(Text, BigInteger)](jsonobject-replace-string-biginteger-method.md)|Replaces the value of the property with the given key with the new value.|
|[Replace(Text, Decimal)](jsonobject-replace-string-decimal-method.md)|Replaces the value of the property with the given key with the new value.|
|[Replace(Text, Duration)](jsonobject-replace-string-duration-method.md)|Replaces the value of the property with the given key with the new value.|
|[Replace(Text, Date)](jsonobject-replace-string-date-method.md)|Replaces the value of the property with the given key with the new value.|
|[Replace(Text, Time)](jsonobject-replace-string-time-method.md)|Replaces the value of the property with the given key with the new value.|
|[Replace(Text, DateTime)](jsonobject-replace-string-datetime-method.md)|Replaces the value of the property with the given key with the new value.|
|[Replace(Text, Text)](jsonobject-replace-string-string-method.md)|Replaces the value of the property with the given key with the new value.|
|[SelectToken(Text, var JsonToken)](jsonobject-selecttoken-method.md)|Selects a JsonToken using a JPath expression.|
|[Values()](jsonobject-values-method.md)|Gets a set of values of the JsonObject.|
|[WriteTo(var Text)](jsonobject-writeto-text-method.md)|Serializes and writes the JSON data of the JsonObject to a given Text object.|
|[WriteTo(OutStream)](jsonobject-writeto-outstream-method.md)|Serializes and writes the JSON data of the JsonObject to a given OutStream object.|
|[WriteToYaml(var Text)](jsonobject-writetoyaml-text-method.md)|Serializes and writes the JsonObject as YAML to a given Text object.|
|[WriteToYaml(OutStream)](jsonobject-writetoyaml-outstream-method.md)|Serializes and writes the content of the JsonObject as YAML text to a given OutStream object.|
|[WriteWithSecretsTo(Text, SecretText, var SecretText)](jsonobject-writewithsecretsto-text-secrettext-secrettext-method.md)|Replaces the placeholder value in the path with the secret and then serializes and writes the content of the JsonObject to a SecretText.|
|[WriteWithSecretsTo(Dictionary of [Text, SecretText], var SecretText)](jsonobject-writewithsecretsto-dictionary[text,secrettext]-secrettext-method.md)|Replaces the placeholder values based on their paths with the provided secrets and then serializes and writes the content of the JsonObject to a SecretText.|

[//]: # (IMPORTANT: END>DO_NOT_EDIT)

> [!NOTE]  
> For performance reasons all HTTP, JSON, TextBuilder, and XML types are reference types, not value types. Reference types holds a pointer to the data elsewhere in memory, whereas value types store its own data.

## Remarks 
An unitialized variable of JsonObject type represents an empty JSON object. Given a value of JsonObject type, you can check if it is empty by checking that the number of keys in the object is 0.

```
jsonObject.Keys.Count =  0
```

## Related information
[Get Started with AL](../../devenv-get-started.md)  
[Developing Extensions](../../devenv-dev-overview.md)  