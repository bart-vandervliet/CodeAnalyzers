Install .NET 8 SDK
Install .NET 9 SDK

Modify `global.json` in solution root dir to reflect the dotnet version you want to use for this project.

If, for example, you want to use .NET 8.0.404, change `global.json` to

```json
{
  "sdk": {
    "version": "8.0.404"
  }
}
```

If you open a command window and navigate to the solution root folder and run `dotnet --version`, you would get 8.0.404.

Then run `dotnet build`.

When running .NET 8, you'll get a build succeeded message.
When running .NET 9, you'll get a build failed message, suggesting you should enable `GenerateDocumentationFile` and some other stuff.

