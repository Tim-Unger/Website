# GeneratePastAndFuture

## Definition

Generate the specified amount of Airacs in the past and the future from the current Airac

## Overloads

|   |   |
|---|---|
| [GeneratePastAndFuture(int, int)]() | Generate X future Airacs |

## GenerateFuture(int, int)

Generate the specified amount of Airacs in the future from the current Airac

```cs
public static System.Collections.Generic.List<Airac> GeneratePastAndFuture(int amount)
```

## Parameters

```pastAmount``` int

The amount of Airacs in the past to generate

```futureAmount``` int

The amount of Airacs in the future to generate

## Returns
List\<Airac>

The collection representing the result

## Exceptions

InvalidDataException

The ```amount``` was not positive or 0