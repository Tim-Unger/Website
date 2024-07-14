# GenerateSingle

!!! warning
GenerateSingle is deprecated, please use [GenerateByIdent()](./GenerateByIdent.md) instead
!!!

## Definition

Generate a single Airac by the specified Ident

## Overloads

|   |   |
|---|---|
| [GenerateSingle(string)]() | Generate a single Airac by the specified Ident |

## GenerateSingle(string)

Generate a single Airac by the specified Ident

```cs
public static AiracGen.Airac GenerateSingle(string ident)
```

## Parameters

```ident``` string

The ident of the Airac to generate

## Returns
Airac

The Airac representing the result

## Exceptions

InvalidDataException

The ```ident``` was not  a number or four letters long

KeyNotFoundException

the ```ident``` was not found in all possible airacs