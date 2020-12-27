### Visual Stidio code needs C# dependencies Downloading package 'OmniSharp for OSX' (49987 KB)


### Create your app using dotnet terminal command
```dotnet new console -o nameOfApp```
- the dotnet new console <- creates a new console app 
- ```-o``` parameter creates a directory giving it the name of yur new app

## navigate to the new directory created by previous command
```cd myApp```

## The main file in the app is a directory created by a program file with file extension .cs
## run your app with terminal command 
```dotnet run```

### Install ML.NET CLI
The ML.NET command-line interface (CLI), provides tools for building machine learning models with ML.NET.

Note: ML.NET CLI is currently in Preview.

Once you've installed the .NET SDK, open a new terminal and run the following command:
```dotnet tool install -g mlnet```

### I ran into this issue:
``` ~/.dotnet/tools/mlnet
It was not possible to find any compatible framework version
The framework 'Microsoft.NETCore.App', version '3.1.0' was not found.
  - The following frameworks were found:
      5.0.1 at [/usr/local/share/dotnet/shared/Microsoft.NETCore.App]

You can resolve the problem by installing the specified framework and/or SDK.

The specified framework can be found at:
  - https://aka.ms/dotnet-core-applaunch?framework=Microsoft.NETCore.App&framework_version=3.1.0&arch=x64&rid=osx.10.15-x64```
  ### this is how I fixed it
  ```dotnet --info```

It was not possible to find any compatible framework version
The framework 'Microsoft.NETCore.App', version '3.1.0' was not found.
  - The following frameworks were found:
      5.0.1 at [/usr/local/share/dotnet/shared/Microsoft.NETCore.App]

You can resolve the problem by installing the specified framework and/or SDK.

The specified framework can be found at:
  - https://aka.ms/dotnet-core-applaunch?framework=Microsoft.NETCore.App&framework_version=3.1.0&arch=x64&rid=osx.10.15-x64
