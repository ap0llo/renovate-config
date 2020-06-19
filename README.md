# renovate-config

Configuration preset for [Renovate Bot](https://docs.renovatebot.com/config-presets/) that extends the `base` preset.

The preset adds:

- Package groups
   - All `Microsoft.Extensions.Logging*` packages
   - All `Microsoft.Extensions.Configuration*` packages 
   - All `xunit*` packages
   - All `NuGet*` packages
   - `Nerdbank.GitVersioning` and the corresponding `nbgv` .NET tool
- Adjusts subjects of commits and Pull Requests to be slighly more verbose
- Adjusts subjects of commits and Pull Requests to use captialization instead of being lower case only
- Adds a *dependencies* label to Pull Requests
   
