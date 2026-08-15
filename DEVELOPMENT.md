# Desenvolvimento

Este documento é para quem deseja compilar ou contribuir com o **Mechanic Tool — by KitoSoft**.

## Requisitos

- Windows 10 ou 11
- .NET 8 SDK
- Visual Studio 2022 ou VS Code com extensão C#

## Restaurar dependências

```powershell
dotnet restore src/MechanicTool/MechanicTool.csproj
```

## Executar em desenvolvimento

```powershell
dotnet run --project src/MechanicTool/MechanicTool.csproj
```

## Build Release

```powershell
dotnet build src/MechanicTool/MechanicTool.csproj -c Release
```

## Estrutura principal

```text
src/MechanicTool/
├── Models/
├── Services/
├── UI/
├── Utils/
├── Assets/
├── Program.cs
└── MechanicTool.csproj
```

## Namespace

O namespace raiz oficial do projeto é:

```csharp
KitoSoft.MechanicTool
```

## Dados locais

Dados pessoais de uso, histórico e backups não devem ser enviados para o repositório. O `.gitignore` já bloqueia os principais arquivos e diretórios gerados localmente.
