# GeneratePast

## Definition

Generate the specified amount of Airacs in the past from the current Airac

## Overloads

|   |   |
|---|---|
| [GeneratePast(int)]() | Generate X Past Airacs |

## GeneratePast(int)

Generate the specified amount of Airacs in the past from the current Airac

```cs
public static System.Collections.Generic.List<Airac> GeneratePast(int amount)
```

## Parameters

```amount``` int

The amount of Airacs to generate

## Returns
List\<Airac>

The collection representing the result

## Exceptions

InvalidDataException

The ```amount``` was not positive or 0