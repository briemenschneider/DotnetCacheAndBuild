# DotnetCacheAndBuild
Action to cache and build a dotnet project

Use as follows:
```
  build:
    runs-on: ubuntu-latest
    steps:
      - name: Get and Cache NuGet Packages
        uses: briemenschneider/dotnetcacheandbuild@v1
        with:
          dotnet-version: '7.x' #Optional, defaults to '6.x'
          with-cache: 'false' #Optional, defaults to 'false', if 'true' requires a package.lock.json file or will fail
          build-path: 'myproject/src'  #Optional, defaults to .
```
