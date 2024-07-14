# GenerateFuture

## Definition

Generate the specified amount of Airacs in the future from the current Airac

## Overloads

|   |   |
|---|---|
| [GenerateFuture(int)]() | Generate X future Airacs |

## GenerateFuture(int)

Generate the specified amount of Airacs in the future from the current Airac

```cs
public static System.Collections.Generic.List<Airac> GenerateFuture(int amount)
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