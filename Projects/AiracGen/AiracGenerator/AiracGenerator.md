# AiracGenerator Class

## Definition

Namespace: AiracGen.Generator\
Assembly: AiracGen\
Source: [AiracGen](https://www.nuget.org/packages/AiracGen)

Provides a static class for creating Airacs.
```cs
public static class AiracGenerator
```

## Examples

```cs
static void AiracExamples()
{
    //Generate the current Airac and print the end date to the console
    var currentAirac = AiracGenerator.GenerateCurrent();
    Console.WriteLine($"End Date: {currentAirac.EndDate.ToShortDateString()}")    

    //Generate all Airacs in the current year and print the idents to the console
    var currentYear = DateTime.UtcNow().Year;
    var airacsInCurrentYear = AiracGenerator.GenerateByYear(currentYear);

    airacsInCurrentYear.ForEach(x => Console.WriteLine(x.Ident));
}
```

## Methods 
|   |   |
|---|---|
| [GenerateFuture(int)](./Methods/GenerateFuture.md) |  Generate X future Airacs |
| [GeneratePast(int)](./Methods/GeneratePast.md) |  Generate X past Airacs |
| [GeneratePastAndFuture(int, int)](./Methods/GeneratePastAndFuture.md) |  Generate X past and y future Airacs |
| [GenerateSingle(string)](./Methods/GenerateSingle.md) |  Generate a single Airac by ident |
| [GenerateByIdent(string)](./Methods/GenerateByIdent.md) |  Generate a single Airac by ident |
| [GenerateMultiple(string[])](./Methods/GenerateMultiple.md) |  Generate multiple Airacs by ident |
| [GenerateCurrent()](./Methods/GenerateCurrent.md) |  Generate the current Airac |
| [GenerateCurrent(string)](./Methods/GenerateCurrent.md) |  Generate the current Airac |
| [GenerateNext()](./Methods/GenerateNext.md) |  Generate the next Airac |
| [GenerateNext(string)](./Methods/GenerateNext.md) |  Generate the next Airac |
| [GeneratePrevious()](./Methods/GeneratePrevious.md) |  Generate the previous Airac |
| [GeneratePrevious(string)](./Methods/GeneratePrevious.md) |  Generate the previous Airac |
| [GenerateByYear(int)](./Methods/GenerateByYear.md) |  Generate all Airacs in a year |
| [GenerateBetweenYears(int, int)](./Methods/GenerateBetweenYears.md) |  Generate all Airacs between two years |
| [GenerateBetweenYears(int, int, boolean)](./Methods/GenerateBetweenYears.md) |  Generate all Airacs between two years |
| [GenerateBetweenYearsSorted(int, int)](./Methods/GenerateBetweenYears.md) |  Generate all Airacs between two years and sort them into sub lists for each year |
| [GenerateBetweenYearsSorted(int, int, boolean)](./Methods/GenerateBetweenYears.md) |  Generate all Airacs between two years and sort them into sub lists for each year |
| [GenerateForYearsUnsorted(int[])](./Methods/GenerateForYears.md) |  Generate all Airacs for the given years |
| [GenerateForYearsSorted(int[])](./Methods/GenerateForYears.md) |  Generate all Airacs for the given years sorted into sub lists of each year |