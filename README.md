# Play.Common
Library for shared code between Play Application

## Create and publish package
```powershell
$version="1.0.8"
$owner="alvperagu-dotnet"
$gh_pat="[TOKEN HERE]"

dotnet pack src\Play.Common\ --configuration Release -p:PackageVersion=$version -p:RepositoryUrl=https://github.com/$owner/Play.Common -o ..\packages

dotnet nuget push ..\packages\Play.Common.$version.nupkg --api-key $gh_pat --source "github"

```