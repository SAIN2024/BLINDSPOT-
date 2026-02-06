# BLINDSPOT 

Multi-project C# artifact implementing:

1. Static analysis + constraint extraction (PLC/ESD/operator abstractions)
2. Trace analysis (partitioning, slack trajectories, recovery bounds)
3. Incident template generation (constrained, safe synthetic proposer)
4. vPLC-style deterministic execution
5. Recovery classification (safe/infeasible/unsafe)

## Build
```bash
dotnet restore BLINDSPOT.sln
dotnet build BLINDSPOT.sln -c Release
dotnet test BLINDSPOT.sln -c Release
```

## Run
```bash
dotnet run --project src/BLINDSPOT.Cli -- --out artifacts/run1
```


## .NET Dependencies

### Required SDK
- **.NET SDK 8.0** (or newer 8.x)

Check installed version:
```bash
dotnet --version

