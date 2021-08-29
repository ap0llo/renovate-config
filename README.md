# renovate-config

Configuration preset for [Renovate Bot](https://docs.renovatebot.com/config-presets/) that extends the `base` preset.

The preset adds:

- Package groups
   - All `Microsoft.Extensions.Logging*` packages
   - All `Microsoft.Extensions.Configuration*` packages 
   - All `xunit*` packages (except `xunit.runner.visualstudio` because that package is versioned independently)
   - All `NuGet*` packages
   - `Nerdbank.GitVersioning` and the corresponding `nbgv` .NET tool
   - All [`Statiq`](https://www.statiq.dev/) packages
   - All [`ReportGenerator`](https://github.com/danielpalme/ReportGenerator) packages 
   - All [`Libman`](https://docs.microsoft.com/en-us/aspnet/core/client-side/libman) packages
- Adjusts subjects of commits and Pull Requests to be slighly more verbose
- Adjusts subjects of commits and Pull Requests to use captialization instead of being lower case only
- Adds a *dependencies* label to Pull Requests
- Adds the name of the dependency as well as the previous and new version to the commit message body
- Disables the "Dependency Dashboard"
