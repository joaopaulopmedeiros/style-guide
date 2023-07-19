# Style Guide

## Variáveis

Prefira declarar os tipos de variáveis de forma explícita.

❌ BAD
```C#
var result = "mystring";
```

✅ GOOD
```C#
string result = "mystring";
```

## Namespaces
Prefira usar namespaces com escopo de arquivo.

❌ BAD
```C#
namespace SampleNamespace
{
    class SampleClass
    {
        public void SampleMethod()
        {
            System.Console.WriteLine(
                "SampleMethod inside SampleNamespace");
        }
    }
}
```

✅ GOOD
```C#
namespace SampleNamespace;

class AnotherSampleClass
{
    public void AnotherSampleMethod()
    {
        System.Console.WriteLine(
            "SampleMethod inside SampleNamespace");
    }
}
```

