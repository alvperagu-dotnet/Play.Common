# Play.Common
Library for shared code between Play Application

## Create and publish package
```powershell
$version="1.0.8"
$owner="alvperagu-dotnet"
dotnet pack src\Play.Common\ --configuration Release -p:PackageVersion=$version -p:RepositoryUrl=https://github.com/$owner/Play.Common -o ..\packages

```