# Nerdbank.GitVersioning-Sample

A sample of how easy it is to adopt Nerdbank.GitVersioning to solve your versioning problems. The sample also includes how to enable GitHub sourcelinking and how to build symbols. It also uses GitHub actions for building and deploying to GitHub packages registry. 

## Create the NuGet

Run the command 
```bash
dotnet pack -c Release
```

The published NuGet package and its symbols will be under `Artifacts/Release`

## Explore the NuGet

You can use https://github.com/NuGetPackageExplorer/NuGetPackageExplorer to explore the NuGet package. 

![Screenshot from NuGet package explorer](nugetExplorer.PNG)

## Build and deploy

This example also uses GitHub actions and GitHub packages. See [./.github/workflows](./.github/workflows) for reference.

## Useful links

* https://github.com/NuGet/Home/issues/8580
* https://github.com/NuGetPackageExplorer/NuGetPackageExplorer
* https://docs.microsoft.com/en-us/dotnet/standard/library-guidance/versioning
* https://docs.microsoft.com/en-us/dotnet/standard/library-guidance/sourcelink
* https://docs.microsoft.com/en-us/dotnet/standard/library-guidance/publish-nuget-package
* https://github.community/t5/GitHub-API-Development-and/GitHub-Package-Registry-NuGet-400-Bad-Request/m-p/38861/highlight/true#M3547
* https://help.github.com/en/actions/automating-your-workflow-with-github-actions/authenticating-with-the-github_token
* https://help.github.com/en/github/managing-packages-with-github-packages/configuring-dotnet-cli-for-use-with-github-packages#authenticating-to-github-packages
