# MetarSharp

## Metar Decoder for C# [[GitHub]](https://github.com/Tim-Unger/MetarSharp) [[NuGet]](https://www.nuget.org/packages/MetarSharp/)

**Library that is able to parse almost every metar, also allows creation of a JSON and Readable Report**

```cs
using MetarSharp;

[...]

var metar = ParseMetar.FromString("EDDF 121950Z AUTO 28012KT 9999 FEW045 17/12 Q1011 NOSIG");

var json = metar.ToJson();

//Result
/*
[
  {
    "metarRaw": "EDDF 121950Z AUTO 28012KT 9999 FEW045 17/12 Q1011 NOSIG",
    "airport": "EDDF",
    "reportingTime": {
[...]
      "reportingTimeZulu": "2024-07-12T19:50:00"
    },
    "isAutomatedReport": true,
    "wind": {
      "windRaw": "28012KT",
[...]
runwayConditions": null,
    "readableReport": "Automated weather report for EDDF. 
    \nReported today at 19:50 UTC\nWind: 280 Degrees 12 Knots
    \nVisibility: 9999 Meters\nFew Clouds at 4500 f\nTemperature: 17°C (62.6°F) Dewpoint: 12°C (53.6°F)
    \nPressure: 1011hPa (29.85inHg)\nTrend: No significant change\n",
[...]
  }
]
*/
```