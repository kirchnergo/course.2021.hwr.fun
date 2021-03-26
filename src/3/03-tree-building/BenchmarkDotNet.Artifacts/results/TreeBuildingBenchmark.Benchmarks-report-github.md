``` ini

BenchmarkDotNet=v0.12.1, OS=macOS 11.2.2 (20D80) [Darwin 20.3.0]
Intel Core i7-7920HQ CPU 3.10GHz (Kaby Lake), 1 CPU, 8 logical and 4 physical cores
.NET Core SDK=5.0.101
  [Host]     : .NET Core 5.0.1 (CoreCLR 5.0.120.57516, CoreFX 5.0.120.57516), X64 RyuJIT DEBUG
  DefaultJob : .NET Core 5.0.1 (CoreCLR 5.0.120.57516, CoreFX 5.0.120.57516), X64 RyuJIT


```
|   Method |      Mean |     Error |    StdDev |    Median | Ratio | RatioSD |  Gen 0 | Gen 1 | Gen 2 | Allocated |
|--------- |----------:|----------:|----------:|----------:|------:|--------:|-------:|------:|------:|----------:|
| Baseline | 10.113 μs | 0.1998 μs | 0.3849 μs | 10.074 μs |  1.00 |    0.00 | 3.6163 |     - |     - |   14.8 KB |
|     Mine |  6.539 μs | 0.2335 μs | 0.6812 μs |  6.354 μs |  0.63 |    0.06 | 2.0828 |     - |     - |   8.52 KB |
