# GenerateByIdent

## Definition

Generate a single Airac by the specified Ident

## Overloads

|   |   |
|---|---|
| [GenerateByIdent(string)]() | Generate a single Airac by the specified Ident |

## GenerateByIdent(string)

Generate a single Airac by the specified Ident

```cs
public static AiracGen.Airac GenerateByIdent(string ident)
```

## Parameters

```ident``` string

The ident of the Airac to generate

## Returns
Airac

The Airac representing the result

## Exceptions

InvalidDataException

The ```ident``` was not a number or four letters long

KeyNotFoundException

the ```ident``` was not found in all possible airacs