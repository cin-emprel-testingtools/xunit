## About This Project Prerequisites

This project contains the Visual Studio runner for xUnit.net. It supports the built-in Test Explorer feature in Visual Studio 2022 Community Edition 16.10 and later. It supports .NET 6.0, .NET Framework 4.6.2, Windows UWP 10.0.16299). It can run tests from xUnit.net 1.9.2 and later.

## Debugging

Debugging the VS Adapter is tricky. You'll currently need to build your own test adapter NuGet package using `build.ps1`, `build.ps1 Packages` first to ensure you have local symbols. The symbols are not in the public package. It's helpful to add it to a local `\packages` directory and then use an entry like `<add key="Local Packages" value=".\packages" />` in your `NuGet.config` file to point to it. Don't forget to eventually delete it from your global profile `.nuget\packages\xunit...` when you're done.

With that as the startup project, you can set breakpoints and then hit them. You may need to manually load symbols the first time if it's not detected automatically.

## About xUnit.net

[<img align="right" src="https://xunit.net/images/dotnet-fdn-logo.png" width="100" />](https://www.dotnetfoundation.org/)

xUnit.net is a free, open source, community-focused unit testing tool for the .NET Framework. Written by the original inventor of NUnit v2, xUnit.net is the latest technology for unit testing C#, F#, VB.NET and other .NET languages. xUnit.net works with ReSharper, CodeRush, TestDriven.NET and Xamarin. It is part of the [.NET Foundation](https://www.dotnetfoundation.org/), and operates under their [code of conduct](http://www.dotnetfoundation.org/code-of-conduct). It is licensed under [Apache 2](https://opensource.org/licenses/Apache-2.0) (an OSI approved license).

[<img align="right" width="100px" src="https://dotnetfoundation.org/img/logo_v4.svg" />](https://dotnetfoundation.org/projects/xunit)

xUnit.net is a free, open source, community-focused unit testing tool for the .NET Framework. Written by the original inventor of NUnit v2, xUnit.net is the latest technology for unit testing C#, F#, VB.NET and other .NET languages. xUnit.net works with ReSharper, CodeRush, TestDriven.NET and Xamarin. It is part of the [.NET Foundation](https://www.dotnetfoundation.org/), and operates under their [code of conduct](https://www.dotnetfoundation.org/code-of-conduct). It is licensed under [Apache 2](https://opensource.org/licenses/Apache-2.0) (an OSI approved license).

For project documentation, please visit the [xUnit.net project home](https://xunit.net/).

* _New to xUnit.net? Get started with [.NET Framework](https://xunit.net/docs/getting-started/netfx/visual-studio), [.NET Core](https://xunit.net/docs/getting-started/netcore/cmdline), and [devices](https://xunit.net/docs/getting-started/uwp/devices-runner)._
* _Need some help building the source? See [BUILDING.md](BUILDING.md)._
* _Want to contribute to the project? See [CONTRIBUTING.md](.github/CONTRIBUTING.md)._

[<img src="https://raw.github.com/xunit/media/main/powered-by-ndepend-transparent.png" title="Powered by NDepend" width="142" />](http://www.ndepend.com/)
