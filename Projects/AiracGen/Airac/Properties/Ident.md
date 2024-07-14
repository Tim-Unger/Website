# Ident

Gets or sets the four number long ident of the airac

```cs
public string Ident { get; set; } = DefaultAirac.StartIdent;
```

## Property Value

string

the ident of the airac

# Remarks

The Ident is always four digits long and made up the following:\
The first two digits are the year of the airac, prefixed with a zero if \< 10 **(2002 > 02, 2024 > 24, 1995 > 95)**
The other two digits are the number of the airac in the current year, prefixed by zero if \< 10, so **the first airac will be 01, the tenth 10**