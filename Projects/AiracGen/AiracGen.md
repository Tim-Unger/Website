# AiracGen

## Airac Generator for C# [[GitHub]](https://github.com/Tim-Unger/AiracGen) [[NuGet]](https://www.nuget.org/packages/AiracGen)

**Library that let's you create Airacs**

### Using C#
```cs
using AiracGen;

[...]

var currentAirac = AiracGenerator.GenerateCurrent();

var airacsThisYear = AiracGenerator.GenerateByYear(2024);
```

### You can also call my API

```bash
curl api.tim-u.me/airacs
```

Result:
```
[
  {
    "ident": "2301",
    "startDate": "2023-01-26",
    "endDate": "2023-02-23",
    "numberInYear": 1
  },
  {
    "ident": "2302",
    "startDate": "2023-02-23",
    "endDate": "2023-03-23",
    "numberInYear": 2
  },
  [...]
]
```